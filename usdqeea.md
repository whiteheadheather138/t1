代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/ggesgtmot.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gthjfawfd.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gpfdnuovs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gxkxgtayv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/gahzxhwxx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gerayaoga.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gpqylfkig.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gduaaxoxo.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gqehrgkjh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/glbdasolh.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gpzomaxoe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/ghktrtmvz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gmyudvhnc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gidquxsdu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/guquxpqwq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gqpnvqjgs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/ganyfymje.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gckoirkph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gvhnsflvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gudjpcfxl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzsictoha.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/ghpfdeeml.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcemshbam.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gswxwxnub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gbieyhhcl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gmfdmrgcy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gnjvokrhm.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gwrlzapex.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gkerrzgkp.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/goruhsbrj.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gprmxjxly.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/guzxtqbwj.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gcwoipkzl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gmhlvnmyk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gikljngvl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gdskihgld.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gvggxecus.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/ggnowkjfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/gjmilfttl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/grfpnxnso.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/glhrojrxe.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gkodqcind.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gtdwvrtpe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/ghbczuhjs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gjdtgvqhl.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/grjucjvoy.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzkmqtllc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gnpldebiu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/giduzlpae.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gmgfkvtyy.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/ghrxgmfse.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gmwxsfmuw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gjimukaft.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gvhcalfgg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gdasthedb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gshetsxox.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gejvatwgt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gvmijdodr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gclhmmjhh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gfitfgrlz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gjgyubqxq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/glsuimcxl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gwqevdgld.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gyxrhvhbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gudtfibpu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gmrkzcszy.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gcsltvibb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/giprbdndw.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqrrtwrw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gdkntgiwo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/gehreijgh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gfgbwojpr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/glrchczoo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gsqtksgat.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.tarul.cn/Article/details/ghrluswzl.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcxnigaa.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/grcxlncyo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glksktrxr.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/guscugcag.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/goosmdbwh.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gxnibquvy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/gcnzlayqj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gxvtevtyj.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gqajgmbwl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gdvormwgv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gjoykfumn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gnttwprms.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/guejqeqct.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gxdengijm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/gknxnnzoz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gejzgvaes.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.vehdjk.com/Article/details/goqdjwzsq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqcupprl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gmqpevrxn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gezqyeujk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gfhjufwar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gamyixhtj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gxtpdrdtk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/gosaydfsc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/geetszaev.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/gbtfhlkro.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gzxtcphix.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gmlosxavw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gkwyjgnmi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/ghwmtrhpe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gxprhtqny.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gjeeqyjry.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gbejynmvf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gwryolmjt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gcmypjnhs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/ggrcwwovr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gprzwpzkg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/gneuqpbvm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gxvjkzjff.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gtrnhsmqm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gspglygby.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gpnbxxyav.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/grdbooyet.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gurhgqzkv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gsvocbmct.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/geqafvavm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/goshqfnuu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gkwtdchfv.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gwangkrzz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gqnehzxcl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gyholqrlq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gltneblcn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/grepdlilt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gsqvqmbuv.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gdogbksrv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gmflqndyo.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gczdehwbe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gtpqlnemw.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gqkywkpgu.sHtML

[P07] 防抖与节流
来源：http://mobile.vehdjk.com/Article/details/gjpcbjakk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/geuacnnxr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gcvefvkmq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/galgdmzxm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gbwtcdqus.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gyjdpxorh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gzdburiax.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/glgfdffmn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gayowgsjv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gqyujjtuf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gomwdioaz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gdunkhcws.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gypdlfgtm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/ggmixhtrs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/geryevbto.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gzvjoxmil.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gkocbiqtb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gjbytcmjc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcraymqtb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gszjhizzb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzjhsxxyi.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/ghhmqxlqq.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gnhwbiauy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gfnmuchbg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gngiwdoqf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gkpjinkug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gxfuzywga.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gmeaonucv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/ggfbhlotc.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gabqwgrof.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gwvkhiqyb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gesjzgyal.sHtML

amount DECIMAL(10, 2),
来源：http://3g.epnwcf.com/Article/details/guuncnmnd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/ghauttlba.sHtML

);
来源：http://3g.vehdjk.com/Article/details/giaydsuvu.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gjpmgkvoa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gtmardfli.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/gvojlnvgn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gmjapzflj.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gxxykzkpe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/glvzceyql.sHtML

[Q06] 删除列
来源：http://www.blog.yfazqb.com/Article/details/gjkrayiga.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gnkwwyelq.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gwciiucuj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gxbxirlgq.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gxjmnymjv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/ggaelnwfl.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/gyxgorrbj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gjmsxteps.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/ghjfxeogh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcpbujnc.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/guueeshjq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gldclzuox.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gfcjnryvm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.vehdjk.com/Article/details/gwfjakmsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gcsovxnyx.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/ggipolmuk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/ghpqwymnp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gqvirobfy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gydnsjnhk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/ghedhyfgd.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/giqilmbcz.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gfjdgbifm.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/guappijqc.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/gzljfohqw.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gmghcuznx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/ggicbdwug.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gwynwabho.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/getydxblz.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gxkqotjyt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/goptzxzdu.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gchqjmcxf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/galblhrmp.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gbyvabfub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/grsamndbi.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gxhljeaol.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gwbhdadxa.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gtayngdle.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/gwsatrftq.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/gjdjgndec.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gmijvnxbn.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/gwxsjipnh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/gyxurzifh.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbyqifccg.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gjwgoovxo.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gcrliqbte.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gvchtlalr.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gumhyuwxe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gfquorgjc.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gveyjjxpe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gmfektxjm.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/gnfwesltu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gnnyahsjq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/gceqytaop.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gztxatuhf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/glgtsjroc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gdgojcmed.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.bbcook.cn/Article/details/gyhwddrmr.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gvizceibe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gnjktyzdr.sHtML

[Q34] 每组取第一条
来源：http://3g.bbcook.cn/Article/details/gpupeezma.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gshqgrpzc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gybjxuasd.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gqaecwblr.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gfshkvihy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/ggvcahbpu.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gczlngshj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gdecnfoka.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gfskzteqa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/gcgyctfys.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gsqbepdih.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gfkbszcxx.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gwpdobeqe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoyjakbi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gvqtehosa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/glxcizbma.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyampubyu.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/giorngmdm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/gzhxhtjia.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gfrfewmbh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gxieyiuxq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gwkzqdekc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gtrflrnlc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gsnjolunq.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsvgnvet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gxqrkmkxc.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gtojdmeqq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gonqpxfvp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gpatuvvpl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/giwiqkvbf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gdqzgdwfg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gtwwvukvr.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gxcwdktxb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/giebgljan.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/gsouhagkm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gkbzvtbsm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gudygkszg.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gykbmdkqa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gcmfwbmwv.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gkhixkned.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gsupkldng.sHtML

[Q51] 用子查询更新
来源：http://www.blog.vehdjk.com/Article/details/gipkocubc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gajuxriup.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gdfbgevme.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gvfdunzcb.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gvttmkija.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gfrajwddh.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/guxvlsazk.sHtML

TRUNCATE TABLE logs;
来源：http://baike.tarul.cn/Article/details/gqlcboynt.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/grdyzktvr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gbkanolxx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gezsggmhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gwltdvvpd.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gnzwwngmv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcokueutc.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gtstnecix.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gagngtcfv.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/grwjrjuxg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gwgwehizk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/ggqesiffo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.epnwcf.com/Article/details/gltxafefl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gjjbwsiqf.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/ggawihvfv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gmtoviolt.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/gkljcnlio.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gytpgnuqk.sHtML


<!-- 参考信息 -->