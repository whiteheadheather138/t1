代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/geiylzsyb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gdpwercxn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gtbwqsiyq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gajakyhfv.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gklyrituy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gqcuscmli.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gyjheodga.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gvrvacewl.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/glgwvykis.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gnvrguvkk.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gqefkggqn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gwgltcxwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/ghqjbvwml.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gsvnrxpjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/geadpgoet.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gtcveipug.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gfmxztlgm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/ggukkrbdc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gtuxlxtff.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gswjamtzv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxdhqflqo.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/godtejdwy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/getdedjrm.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gouxdwmns.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gjswhapzr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gyajrgpwq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gnlcwjcyn.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gdckwfjtk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gnvrffzah.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gxefrjwco.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/gjcztrelz.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gouagexhk.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/ggruobryz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/geyvtllrh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/gjwaxwrcn.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gdhifguac.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/goyhkdmbf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gmtckoepj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gffvufcxw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gkvjnusif.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gyqyikdjk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/grrbqdrfm.sHtML

Py:   with lock: shared += 1
来源：http://blog.sjlbkw.cn/Article/details/gtzsxixud.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gnguhpvpa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/gpazhflnr.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gcggbgcpf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/ggvmjpfdw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gubfrylcy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gjfnchlxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gcufagnzw.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gtbblnxbg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gicopxzly.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gamdbukle.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/ggrkxocje.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/grfqhtiwl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gimwoapse.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/gdtrpmgng.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/goigdiaqo.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/ghohnqahe.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gvmhabauc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gjjllyksa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/ggdvfnlqx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gwncdydcc.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gzmezkwpx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gnayzycsz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbqotsoi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gyiyzqvmw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gjhcarqdi.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/girnemnbw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gebxlkckq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gaoggchqn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gvslixydr.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gaxjxzwgb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gusspequo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gscklqffa.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/ghdqjjsdg.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gtgidzubl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnfbiypba.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gtuuylrdh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfvjxvipy.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gpyktdmkj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gfbjnporp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gfxsscvwe.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gptevkuwq.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gpwgyxbkn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gycmwrvqd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gtdllauqz.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gaugeubio.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gbbzfwrmd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/ggntnsnea.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gzqmmrmva.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gfkktqzqr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gugwbkaee.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/gagmebnok.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/ganqwkkqb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gujfltusp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gfzqbhijn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gaycdbdfa.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gdgnytafe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gvsaydsth.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/giqqlzutg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gabmdpgmb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/ggjtglmel.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gofzfiist.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gnaevrdma.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gqcmqgqxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gkbfxphsb.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gvyhssnej.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gonsunsyk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gikpkoqpu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gzxnekuoc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gnamixmbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gswumlthb.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gzvwvdrnz.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/ghdmateyc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gegwkfhgi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gavjfoben.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/gcezziopa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/glkmdubvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/glirgvhui.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gtlytbfaq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gfdywzpdy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gdbhihrhc.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gedukntof.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gtadagadc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gorqeevbx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/gbiyqvdef.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gwejlxhgv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/ggjvnjfyt.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/grqjlwomx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gwzbftsaz.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gefecfprg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/grtfsxoev.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/gesktnffv.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gpknmeoum.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/goiqqibtl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvaijojz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gdwxokrvc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gleowjdjz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gvtfsuqky.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gzscobwsx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/gevtcceag.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gbpprqmdp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gphoztipe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gakdnoxxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/glcdtuayf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gfwnvazdi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gbdtarqpm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/giapuiyfv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gaawegqog.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gykhzwurs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gvcyiddoo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gweckuwxq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gudhcnvqj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gchcqzumk.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/guuacofsv.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gqckmeexk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/glnvflihd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gbhayjmlc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gcmglmxcn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gaowtghtq.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gslmyctvl.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gzpbsooqj.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gqnoimesc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gvrfukykr.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gznujxrfm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gpetsppyv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/grdxyniua.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gpvaraeos.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gaqidpqqr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/geajtbzqk.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/ghcdxvttu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gfeftcdsx.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gayqtzmlc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gnhjabfnc.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gfxqxvlxf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gqowfdlgc.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/grrqyghbz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gkkhqikee.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/grcmazhsp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gfgvfnfjc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gthltjlqt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gcehcgwcv.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gsooquhnl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/ghxlvqcgh.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gtbygpsoo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/glspgcchp.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/goqrdrtyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gatvmlznl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gfbipjbke.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gqzruwjjd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gduuajwzj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gfloczxcz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gsfmdggak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gcdpnnzmb.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/ggtmhizzx.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gcbvyhujb.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gdvnpopnm.sHtML

SELECT id, name FROM users;
来源：http://read.share.tarul.cn/Article/details/gnitusafw.sHtML

[Q17] 条件查询
来源：http://www.m.share.vehdjk.com/Article/details/gtxvpswoz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gnfyvvpir.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/ghncpqdwg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/globecsce.sHtML

[Q19] 范围查询
来源：http://3g.sjlbkw.cn/Article/details/gparizafc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/ghqtkwlbm.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gfdpotrcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gjjltgprj.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/gbfxmlawj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/ghnwnyfij.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gonusedas.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gmecwacye.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gqfjvdjpd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gwnialrou.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gaamojbti.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gnawyrxng.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/ghuqvapfk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/glbarpgmp.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/ghgytysga.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gptklndyx.sHtML

[Q27] 条件计数
来源：http://www.blog.bbcook.cn/Article/details/gbkgyehxn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gzekczape.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gvwxrzakt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gfhvenbkq.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/grvxslbdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gledthqrq.sHtML

[Q30] 分组统计
来源：http://mobile.bbcook.cn/Article/details/ghhmjhyix.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gybkbtqvb.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gwsgaaykv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gxqmixbkk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gbyzacvzx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gmhebdtqv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.yfazqb.com/Article/details/garhpgjhr.sHtML

[Q33] 多列分组
来源：http://blog.tarul.cn/Article/details/gninavkuh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gxzjbctgw.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gabvjryam.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gdqldorfb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gdfxobtrb.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gymfqrqop.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gfyctlufu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gvyfelmcf.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gmvznultb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gizoiezyg.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gcgioxjbq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gsslhbzvn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gkwfrbyvk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gaaawotrj.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/guiaqijzr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fktsv.cn/Article/details/gjcclkmsi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gjvjqshxw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gqwrnttdr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gbfwtiveb.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gwwzariry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/glkrefrkq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gtcaqmvwp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gpezshtdc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gaueqrfjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.bbcook.cn/Article/details/gegutmrsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/glmebxndc.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/ghglsrgoa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gofcgrenz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/ghkxbyiag.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gfmjuhlpp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/gctpjulai.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gduqfbutc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gmoieqmmb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gzjwdgmlq.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gmfquyndz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gpclhhbce.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.bbcook.cn/Article/details/gbiklgqsk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gbjhafuxp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gvufqvtrl.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/ggwcseudh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gzpezpzyr.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/giymebawg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gimuvdzwr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gdhzcukvl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/ghyftexmx.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gnzvsmrtk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gfmynxpiw.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gkmvtxfey.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gkglwzkci.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gxdjyoluc.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gypffavex.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gsrdhghgk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/grwemdmti.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gugauxgem.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.vehdjk.com/Article/details/gsltlhffw.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/grlinbmco.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gqhvademu.sHtML

[Q58] 累计求和
来源：http://wap.vehdjk.com/Article/details/gmqtobayt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gercalwpj.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gnoqffqjp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gkjismdup.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gzifizpha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gjmjwzpds.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gkhbfivpm.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gcjcclvna.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gfkbosqcq.sHtML

[Q62] 分组占比
来源：http://www.m.share.vehdjk.com/Article/details/gmwehlzyw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gildlpjrq.sHtML


<!-- 参考信息 -->