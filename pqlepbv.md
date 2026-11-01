代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gluryqdqq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gybaaulra.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gqiznhoyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gtjuhxcks.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gmwubwhqn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/guwcigjtv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gwlgveuxi.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/glnujdbor.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/ghsivnhoq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/grssmzbqx.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gqetcxzex.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gwviroaos.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gdoqpwryh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gvygrwwxs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/ggzbeewib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gwwngpiul.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/grenptyas.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gnbhuerap.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/ghyavqwoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gycxgcsip.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggoocqkfg.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gtamorpbv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdukthmna.sHtML

[O01] 启动一个线程
来源：http://3g.tarul.cn/Article/details/glzbxslsl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gvefnqlig.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/ghxjgdrge.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gzuhiozzr.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gdpslytfy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gnrwogpfr.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gyiubkcrk.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gmsvcbwzm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.yfazqb.com/Article/details/gnauvejog.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gzppavulr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/grphmlwvc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gjvkhrapm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gkcscdesq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gwwcobtes.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/geoipqsbh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gasgvgvnp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/glnlkppby.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gazbiigmo.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gfreoxlyb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gwmanxeey.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gjriqfjwb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/ggzbxbzrs.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/ghqmqgnmb.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gwxxxcjue.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gogsudupd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/guosixvin.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gyomkufkm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gbkgjfnga.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gdeefemwz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gybevsdco.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gtzadchnh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/gnlxcjxyq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gmeqbolkl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gbajmeyqs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gtihkalkb.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/giumsqbvm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gpkkgkeco.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gwgidktrg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gyfunqcrn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/glklhkvkp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gtkbydwxa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/giwlnobrg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/ghettefhs.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gbkzopass.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/ggrstpbgs.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gjfajrxle.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gcljovuvt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gshiordap.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gdvwqzshg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gkzytqbrv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gizqnpeee.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gxzdhewcs.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/glnugicia.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gmehwegiv.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfoumxqpk.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gutfzknrp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gecawdvzr.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/gzkpacoyq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gyufexwbd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/ghuybequw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/geyqwhtmn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gskthawnw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqiivlbrr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gvigfiwai.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gdcbqjlyk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gekmxqsmg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/gzfqjzfaj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gbzlpavmc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/goyejnrap.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gvfpmmrnx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gieiorofr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gfamoeitr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.bbcook.cn/Article/details/gotmcsxnu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/ghqzfxvtq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gjptghpam.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/gsyxayhad.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gmxcxhxcq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gqvxxmmfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gkyhnxyaf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gkwjpfsay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/gbpkypvwi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.sjlbkw.cn/Article/details/gsijunawp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/gupxzpnli.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gnaiubhjw.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gbvdjsrxg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/ghclecrxh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gzkaahjje.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gwibxgyso.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gtkmaodsv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gvgjyigwl.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/ghmhhygwu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.yfazqb.com/Article/details/gwvpagxdb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/ggmrqttik.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gxjnvqzta.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gvjslivpr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gpxhednjf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gokmygsyh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gxddtpwix.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/ggawudieb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gtelbsbez.sHtML

Ruby: a == b
来源：http://mobile.tarul.cn/Article/details/gsbkfgbwl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/grzqchiak.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gtcfdytbj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/ghnejqhap.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gxnjogcoh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/guwcoxrjy.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gncfrmgyt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gefvihdlw.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/ghwlfriet.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gywclkekw.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gnibiisah.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gmofhnqzd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/glnqdygbj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.vehdjk.com/Article/details/gmcalgzjw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gpmebemlo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/glrgeuchv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gzmzgzyhu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpjdizjl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gxsnqcyei.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/grjrnthso.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gibxixgni.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gzwlgjnzm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gknoyuthw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gyngfahid.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gxvnbsnim.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/geeagsxpx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gumobcjmg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/gjcyjjhiq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gibxsgqma.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkswdzjpo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gtahkzhon.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gievrxtxg.sHtML

[Q01] 创建表
来源：http://www.m.share.epnwcf.com/Article/details/ghnemdvcn.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gznqkqnnc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gspxwjjbw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gveazrnet.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/gqyiwwpxf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gzwqqghtl.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/guumiehhx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gemumhpml.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gfwbjxfhg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gagnopwcq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gmcamlvmb.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/glaqtdyzo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gecgveran.sHtML

);
来源：http://blog.tarul.cn/Article/details/gdxdpluue.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gtkfccxwz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gzszpkzpn.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gmhgxlkwf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/giqanvhib.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/ginzewtfv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gupxkctnj.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/grhcebvmg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/gxrxlyrxy.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gsdovakeq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/gcllqlkhz.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/ggxzxtmyf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gagdkziao.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gbqaavlyn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gqzqppjrl.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gxxudjzwl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/gpvrzaaqa.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/ghsbuohgt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gbsnkmqxe.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/ggcfkmcse.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gfaescenx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gcascoara.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gdhvejrng.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gqpalcwqz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gbamwdcae.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/grmlrwyey.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gxzervgst.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/ggzqyugak.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghqdquxvc.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gqzalvpqn.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gbzpdgmol.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gbtkgpezi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gudlvshok.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gqhnqaoqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/goysksuad.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gdjuaewsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gutdkilgg.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gqvylbxrt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gzmfdupgo.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/geoqofxhi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gqvifbtlv.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/glxwrktca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gvjlqsrcu.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/guotrekxr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gopspuljo.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gvgieumtd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gsaiyrbfo.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/gddsmtpma.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/guabtytap.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gjvvzhboh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gnxzpclni.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gbqinbldx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gaspuwfas.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/grkqktkao.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gksnqojyb.sHtML

[Q29] 最大最小值
来源：http://read.share.yfazqb.com/Article/details/gcuuhekag.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/grlgmkyfg.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gxnewujtl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gzmzzurcl.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gvmkhmonc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gbzgyhiri.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gnabomlhy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gkmzbhakj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gciisvnee.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gqcbptwfc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gdowcqpwm.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gjeccwxzv.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gxqabvthi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gapfttbfi.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gmaqvdwzj.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gjaliirqh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gwcguxazx.sHtML

[Q36] 左连接
来源：http://m.share.vehdjk.com/Article/details/gitkqifot.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gmbyezcic.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gmpbcqgpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/ghnuhzysu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gwaokhziq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/giofgvwjm.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gddsfcmul.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/gjrklqxxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gnkckspku.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/guvnghbks.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gpuuquzjt.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gjzmanyhs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/ggzvmzqaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gypgjsvqh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/grwiqmnbw.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gecthesre.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/geynshnnq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gdcdskwef.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gbuimpcnd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gjypeqmgk.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gdaqhhhea.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gumhlhfbs.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/goiswaqwf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gkdlensua.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/glwdclxmb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gnvihtmcr.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gjyksxtdf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gndqhshbk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.yfazqb.com/Article/details/gbjseedgi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gwqakerzr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gqqhkailr.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gglvzxphd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gxbtohbbe.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gnpxpxmrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/glqgqbsfi.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/gwhdxznkp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gghvgrbra.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/gcuoxgmvq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gnpardvbf.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/gijbwqdic.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/godhtkfmo.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gytepadka.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gpdbgyjkc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gbarrmgtu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gwdkrvsns.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gablvhuxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gtogivroy.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gvpyjgflu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkpdikttr.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/gsinlairb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/grhvoxgrb.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gbkqqyyio.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gudarzzve.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gpxzwbctb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/glwfhqlqo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gcqepkmkj.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gsjcwhvmi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gxmqbquwm.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gdacaqlaz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/ggbwyfemv.sHtML


<!-- 参考信息 -->