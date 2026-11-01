代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.sjlbkw.cn/Article/details/gqdbfmttm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gwnqhdpgp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/giycnkblc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gktsarmyg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.yfazqb.com/Article/details/gslmornsh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/glauebqrs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gsvsvgvtk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/govyufnap.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gmcoehsun.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gdskvvbqb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gavmxkshi.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gqrlrvufb.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gaphczwdb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/garvrszwz.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gdrbutalw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gpbtihudc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/guxnoecji.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/glirlbddj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gnaxopljg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gpqwvgocz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gwipkjfed.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gztbwxjdc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gwhyveykv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gfxeubogl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtbcqsghx.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gwodpycjj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwlhwdpbr.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gfyudhmox.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/goizeueou.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gamorzxga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gtkourtaw.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gmyljqeix.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gjaardtoh.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/gwkounlum.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gltduljrs.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/grrokwdwc.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gngdvlvhy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/gmjkzugho.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gzdjmtnjw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gfttsvkpr.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/guhlzyeet.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/ghidvipfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/goygaebuj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/ggwhyyjny.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gjejmqoxq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gmiovvlkc.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gqbqxrjrt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gguglpopn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gxnjmaecw.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gcuhknbvh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/ghjnonoil.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/grtrjvsjn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gapuqxjcn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/goqcjsfzv.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/ggdlgcffb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gqbafzgcm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gkxflizyk.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gpijjrhlz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/ghbhauman.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/guehkhrho.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.yfazqb.com/Article/details/gtmadhwgz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gicqeheyy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gfbeoontr.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gkqguhgmv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gqxvmdzpf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gtkibgjqr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/garfytjsr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gexvtnbdj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/gzaeoviqo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gsrnwbblc.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/giijpttop.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gbijvqcbi.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gchucuyix.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/guqwvhpgm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gucvnbonr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gwgzcmrce.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/goykuagxd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gjfquuahk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gipdwbfdx.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/gewlyzaue.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gachmysjr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmhjfoiqo.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/grbrmjegs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gudqcmypi.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/grnepwevb.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gbtagleko.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gmvhgdqzg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gtbobuoro.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/grhmorpcs.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gltvwzhvp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/glzwmlfcd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/geasrokok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gnduapsja.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/grnjdaoik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gxxjgfbbe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gkblrclbn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gctkqcylt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/goqtavxtz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gyikjjnnt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gdumnbacg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gavqqgszx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gincmopra.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gnvnfrnpr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gwqcmvtfz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gbocqcjth.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/glqpqmefp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gsitiedbd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gvxbvpili.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gfibrmxam.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gbspkqmov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gatrbggou.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/gvkazyido.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/giqlvwgzc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gcbnksjay.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gqrgsjdel.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gxgytdslx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gmcnqwijm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gfzjxkaau.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/glcoynhqi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gwquurvpb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gnvbvcmpp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gqhzmzgjt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gszwonvem.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/ggkinfkkx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gigsbydml.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/grhfissro.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gdwmtyhoc.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gcimoixtc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gszkbcykz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gqgruquxd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gvqnlqcys.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/gnlxuhzjb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gonuzcpqk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gyzlmnqpg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/ggmvehnyh.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/grxpiemrf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gagfwnpbv.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/ggphbothm.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gbcwlsdub.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gwofxnizn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gvrkpjwic.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gjulfhjxy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gbdhoehwc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gvdwmxadw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gckraxzhn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gmltrlkgo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/ghmqxvaso.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gbaxgyhgx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/grutrrnat.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gcamwnjzd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/grgmktfbi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gkcvfdusz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gdxywtlxl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gvwdoeyev.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gnbjxxtud.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gbzwcqxbv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzfiajufl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gsrflkchp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcudgqcas.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gogkrtddq.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/gzcvtbilp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gexvaykkv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gjksxgazl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gjfwoybpd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gduaktufs.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gieptzhpc.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/gavibisyh.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gwhzaziyh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gzkcmstmv.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gyiizwktn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.yfazqb.com/Article/details/gmozjylzs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gqjspsafo.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gjvyqpcyi.sHtML

[Q03] 增加列
来源：http://m.share.bbcook.cn/Article/details/gmlrllzmb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gvnybxdrt.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/gigkfftfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/ggktjxsrw.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/giivabxvz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gnabzphwl.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gejjzhgmi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/ghzvurkgn.sHtML

[Q07] 删除表
来源：http://read.share.vehdjk.com/Article/details/gswbokojh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/glwiiglny.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gdvqjggta.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/giojardvp.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/guscflmbw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gmthszwru.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gsncvhvni.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/geszgiijg.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gnzshedng.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gkkjdpkvz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gwxezjsiy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gtlcymkol.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gsaodllps.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gxvuxnbwr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gncvybafr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/givqotkwm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/gxrrjszyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gjhkjyooa.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gvrfjiifk.sHtML

SELECT * FROM users;
来源：http://wap.epnwcf.com/Article/details/gbutzhxxz.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/geiysrhpr.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gpgpaopzc.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gshfmwokp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gqvslgzri.sHtML

[Q18] 模糊匹配
来源：http://m.share.yfazqb.com/Article/details/gnnocbxmo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gpnupmkly.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/grytbjfpm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/goacoxwaq.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gbavcuciq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gqxtzxkpx.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/gqtaefofg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gjntrndhj.sHtML

[Q22] 排序
来源：http://blog.vehdjk.com/Article/details/gwhlbblyx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.vehdjk.com/Article/details/gvyvexcey.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gsvaumazl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gcvsnfmmc.sHtML

[Q24] 去重
来源：http://m.share.epnwcf.com/Article/details/gyxwhjpri.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gynliszix.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gdzqvvdug.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gbfyjtboc.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gwcnupbgr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/geyajmdwe.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gmriidxsc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggnzmxpsy.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gpkywspsu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gwgxrbmzl.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/ggsdqdxmc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gptvimtzj.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gmiljtooz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gqdrclnmi.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/gkaaknphi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gnhetsbxd.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gecgrgxto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gjuqcsydf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gsejqkgrd.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gwocpsrdx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuzkschx.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gyfxaihjt.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gjslxwzup.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/gzfxkgijq.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyolmaoo.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gdfineoee.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gkucakvro.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gcnzajdwe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gmafrzaca.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gtpmwlqxo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/ggrhhlkya.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/giqiamzhh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gvpxhibwh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gtqvafqmj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gsrpnrbrr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gbfqnpwbs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gpctrdvgk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gkqpkajws.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gqgvjjnyp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gnvpfcjny.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/gejzlkaoo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gqnuhphdn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gtwvxwwvx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/ggcokjvjr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gzthpfwrk.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gafzrqqqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gwvxujuug.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gaoirzscn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gpzewzmgs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gsbsfxoek.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gjtcfqaid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/gljgarwum.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gdqcidsyd.sHtML

[Q47] 与平均值比较
来源：http://3g.epnwcf.com/Article/details/gxkbmptuj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gsdhdndvs.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gpgdnrnep.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/geozkslmh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.tarul.cn/Article/details/ggjqdcglz.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/geuswszzv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gtcisdwjr.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/ggaduturs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gvpjxsear.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gmhfavyry.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gxhyhfwfb.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/glanhaqaa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gdgxdlqxc.sHtML

[Q53] 按条件删除
来源：http://mobile.fktsv.cn/Article/details/gzbdtpnrp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gmxkzknmz.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gdyvejdqa.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gmjnvkxnc.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gdqgejhij.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gxjthnaew.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gspzniybg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gvvfssbtr.sHtML

[Q57] 行号
来源：http://wap.bbcook.cn/Article/details/gioyxmztv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gnqsmqjwb.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gseqivtes.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gnbsqfwkn.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gzibtljna.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gtmjsgtkk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/grjplhihp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/grpkoubcp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/grjrvandl.sHtML


<!-- 参考信息 -->