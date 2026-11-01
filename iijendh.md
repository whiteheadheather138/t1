代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gjogocwto.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/guclvwyac.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/galzrrfou.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gtiosbhmm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gykxvttmi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gaebvchwg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/guwrflhlm.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gqzqezzan.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gvnsvtzog.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/glmifmvef.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gkabmymgo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gtzjhxohv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/ghmukdawq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gzfyapykn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/groaawhet.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gmhmrrzhx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/guvydrurp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/gybooapht.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gqhwrpczj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gdaeqxvnr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbrxicyqj.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gmvbcyvzb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxtmackvl.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/ggscbegah.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/goifwhljl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gtahkhtbj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gtsgfuzsm.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gnxivavzj.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/ggfcsxnax.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/giqziewbx.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gvjsdaeof.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gywdffnkr.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gkvbgzsjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gqyzpnpux.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gknffyqdk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gdsdpfevo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gtuulcxfu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/grlieubfg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/glzxxfods.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.bbcook.cn/Article/details/gstinwljy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gryqijvvn.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/ggmmvbqmd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gxcwizapk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/guibnqiil.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gbwjnoqls.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gmxrbubgp.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gmgzzlqxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gquevauhg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gecvvaklo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggssxtgxz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/ghxqfkfwx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gnxingqfq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gqmxboqpu.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gcuikomfm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gutaxrngr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gttbdsuom.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gcgonldie.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gbxezzamf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gznuyxzss.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/ggdfxvxem.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gnggixmhb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.yfazqb.com/Article/details/gpprxgdeq.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/ggkkbevmw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/guoylfsbh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gczhkgdoh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gvfantczf.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/ghjryjzan.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gredwirpl.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/grdgkkypi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gibggvszb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gcncjlfrj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gwolgovpv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gyuhopzsb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gkxlxpszm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/gyjmyyylz.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/geibmovci.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/ghdtoiftn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gymqupkps.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gaaxiwfex.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbvhnklbr.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/glrqzzbdv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gotwniiol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gatyirnkn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/glyspmvza.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gvstgnsjg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gjacnzayd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gjdfmgevo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gpdgfoxuh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/glhbsvstr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gzfvkrsee.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gltitdlng.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gakjwstng.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gjvcxdxee.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gcukiniar.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gpenedrme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gqhduhhls.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gvdxrjbos.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gkgevtzmg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/grtflwgff.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gvagjfgzo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gsfqpspnn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gzbjyqxtv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gzqapscct.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/glkvtpjvc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/guugswkiq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gwhnouljr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gzzuzvmqk.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/gnxkbqemu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gfyjktekc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gmkmfprbi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gnfonumbo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/giobwbnec.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gylzqviuo.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.vehdjk.com/Article/details/gvmixnnap.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gjjupbaup.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gmgpnpmwv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gheufupyc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gymywottg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gwypxvcxf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/gsfcbvysd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gejptgpdw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/goakgmjfl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gyzhegleo.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gloixykek.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gykphxggo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gwzvppsot.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gwwbhyyje.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/glgdpvrrq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/greggaahp.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/ghnsbxels.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gvtebenki.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gzdvnarqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gxotzeffj.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gtrlneury.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/gwrngccxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gqipsmhmi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/glrqgicun.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gkrpgzwvk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gmitghbaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/gzgbbjblt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gmkrczgyp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/gmghozwmf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gpdoqyfru.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gbubplxaw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gntzbijny.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/galduxabz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/glqohhswn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gychpwdmq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/ghqqcztws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjfwtgbq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gybjdawps.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/goflzqgce.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwdemxukk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/gpsxajzih.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glvczirxo.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gwzufssrm.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/guwtbrsnf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gixranylr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gmgbaswig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/geoolybzz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gicjmerzu.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gwbcvfobl.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gpskozjym.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/ggecxxvje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/ggmwnmsfb.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gqevwuvmb.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/guovgjmyl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gedhkuzzg.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/glfrqmddp.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gqoazpbux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gzyiwqubg.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gucfvmuhl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gqulnbfem.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/gxapfzwdj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/ghjuownul.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gxkhnsncy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gtqamscyh.sHtML

[Q07] 删除表
来源：http://3g.yfazqb.com/Article/details/gtirknbjs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gzaewajop.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gjulaieiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gfdgurkpb.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/govniysyw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gdnmjzphu.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gvruwbgmm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gybkeegzj.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gtsxuoniq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gvwfledqb.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fktsv.cn/Article/details/gndhprmjm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/ghlpdsdid.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gvoasuhjz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/ggjtrhwsu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gdbtcqecg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/goqpkbzzv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gqgvjrgqx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gjzzqxgdo.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gbbytwrah.sHtML

SELECT * FROM users;
来源：http://wap.epnwcf.com/Article/details/gxsmmcgfs.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gmpmcfqfk.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvlxyjrlm.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gyyfawpig.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gcjwbuoff.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/grdnbfgzk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/gtwkmbcpv.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gkbnbhxgp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/grezxbgut.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gqzssyofm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gqprfjfwa.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gjzqyqlrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gclhfvdbo.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gxyiwffab.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/ggerfsuvk.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlyjdtfm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gzsfqgzgg.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gmtbtdroo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtqoowvye.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjstyamb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.sjlbkw.cn/Article/details/glsdbpigt.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/gpnumnmgz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gqcjblxtg.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gnudogvsd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gdxvtyedv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gsspdrakx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gelrrekwn.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gbppzzhhz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gcymkxwqy.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gfudmkzfi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gxxunrcdj.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/gnfnyxlyr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.tarul.cn/Article/details/ggbhgnpij.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gqtywkqhm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gbbrxtktl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gtxgjadkb.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/grmnkfmxq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gbdtouthw.sHtML

[Q34] 每组取第一条
来源：http://blog.tarul.cn/Article/details/gsnddhdur.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gqhgztmrw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gcfsgxqyg.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gxhxgrrrc.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gyvmnfupt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gwknzoxye.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gxoicztga.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gdzmmwmde.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gnklaoahf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gbpnvqvfh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gjoajynyo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gqeuxwkhv.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/grahkzukb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gtqczyoyz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/gxcijbswd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gfigthmjr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gsxsxszpi.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gdemrrrci.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gmmxngkvj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gbauxhoig.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gfekvjqrp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/guiazqqsg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gatiqtocr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gqkmuuuhn.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gadidbvny.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gkssqwyvk.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/gyrdflybk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gkofuqxlp.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gvxzffmit.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gcdtwdbka.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/ggseolmyk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gkjupugzn.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/gxxmlxkvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/gpupvofrl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/gvkiiloge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/gvniyyzne.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.bbcook.cn/Article/details/gpxsywpup.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/giutqbsot.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/ggjgzmasj.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/gzrdprnkt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gotymqubb.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gtytlhqks.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/geebaqrjo.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gkbwgrltz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gfwmrrrap.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gmbsyxial.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/guoclkpbg.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gqhnhjigo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gyxoeiszm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gxhnwaxyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gtbagnoga.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gwfhciwzb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gfmpahwgl.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gyhondhim.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gstnrhlhw.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/gmpkynzsh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gkkqfnozs.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gjejjmnxp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/guvrlxevy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/gvffxjnzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvkbsbsg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gkarrmmlj.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gvpbcackw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gfvzhqrrj.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gvamefary.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gjnrokxtw.sHtML


<!-- 参考信息 -->