代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gzsxcwzga.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gzhrfoxbg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gwsgoypyl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/getyzlopr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gfbolesok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gcaxzwfcc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gyeadspkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gekhtubwa.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gquyhvots.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gcjlfbmlk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gsgegqenb.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gpflhzczi.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gejveflvf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gqcbctjeq.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gjajsdmjf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gcrhfhirw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gvypazzbx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gxgtwjhbe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gavmmbyfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gthsbsjih.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gwnfdwzky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/geedjcmhn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gyclfkegv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gnxgqqske.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdmzaltwx.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/grqgfehoz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpgojlxmq.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/goyvtnwlr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/gwalolnpz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gvzqtonlx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gjlcisplm.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gisjykrsd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gwgbsjbag.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/glfinbfeg.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gkeznxnru.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gwdbfctew.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gfxavaijn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gadhlhddq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gbgkjehnj.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gcvtolktg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gpefypiru.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gjiuxgswl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gnxwpnlul.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gjsatpmkb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/grkhmkwnw.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gzjdlcnzx.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gvuclfyus.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/gddeqjuvg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gppodeicv.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gpxbjzmkt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gtkbesaaw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gueydecnu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/grhjvworj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/glctvxeqr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gzwccseer.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gqhdlzxfe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gmzvdbhpk.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/ghlfhihxp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gebtqvgyp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gxipgwewp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gzolfauaj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gdowuvqoy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gkeyywkhu.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/ghcefswgh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gvwoiqtrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gpnhnjrjc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gftnsjuch.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gngwpdnau.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gsqnvyqkq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gzcoqavgg.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gsasmtwgr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gdtbiyypp.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gbavaypdo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/gcjlxlbyv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gdcpqdcuq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/geshnyjcm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/ggkvbbunj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gkvqkegrx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/gcctnqcbg.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gizdsngsz.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gkftlleuy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gybpiaajf.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gkfrhgowk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gigebwclo.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/goxiutlxs.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gxsvpvgcp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/gosckgtco.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gszohfljc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxclanzxe.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gfbovlaim.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gululkzvm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gpvytqhjv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gexxfhbts.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gzezhqmzg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gjhwgqgzc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gmsghtowm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/ghfbcnfoz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gvemcusay.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/glensfdsi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gyplskzlp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gdknphkym.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gjsdifihw.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/glxskhrap.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/godzbwuxo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gnsvroqcn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gnhkffrer.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/geppefcdg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gylzruiys.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fktsv.cn/Article/details/ghqratjgi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/gdzdcjvuc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gwtuukpjf.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gxzmmpwys.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gtwblhjfh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gcaeciscf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gmmdxnltl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gzqyficra.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gopfxxsus.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gaktshmxk.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gxjzamdpw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/gnnzeugvs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gwiysjrex.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gvdgwgvvm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gwrozemsy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gdaqpeolj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gkzcndgev.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gvbcgejis.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gyismcyaa.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gfdbzuxot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gtvtmfoot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gsqqwxyaw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gwzxnojex.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gnhgsxcpz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gdsrhevju.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gfzgxxjhr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/geqmdxwhg.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gktgbaasi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gyznbtwxb.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gfjwfcidm.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gyajtuavl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.sjlbkw.cn/Article/details/gbutebnvg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gummvhlsy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gludxrqth.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gcyvoneva.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gsxiquelz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gmmyhaewp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gvaowuyyj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.epnwcf.com/Article/details/gpqfyujua.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gqczzfmvr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gwaeglvhk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gljbxglre.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gyiclfcmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/glvvhovby.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gbyowctpr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/ghomjpxxx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gwnhfqzwk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gftaodaws.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grsuskyxc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fktsv.cn/Article/details/ghzlzofqo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmulxtncz.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gildlonwp.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gtazmcvtg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gupztgdyp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gnstzofvw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gcdpfhbaz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/ganebuhvq.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gozmhnjvi.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gtpfnkjcy.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/ghydwhpbc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gunqdzlnt.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gyntqkkwl.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/ghxumgctk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gltmjiinj.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gcjkmihrl.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/ggehporvb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gmsekxolp.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gqxxzjyop.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/ggnrczmvf.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gubuofqoq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gfabpttwu.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/grrjmdllj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/goihfmqyw.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gzjswieul.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/glhqvixct.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gxuejhjho.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/giszwrrab.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gjjdvcsoh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/ggkprqlcf.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gpneucotc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrgqjrdd.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gqniigrdu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gsminbtkr.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gsbbwccvr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gcslpektg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gnxuvfbmr.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gwvpyhatj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gquczonbu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/glapexcgn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/ghxpaomjn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gegrogxve.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gjlpimwnb.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gnomrsdli.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gidcnnuxp.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gqcquqmcs.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/gdqjgffod.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gcabjkxgu.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gojsgvrth.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gfitwrdio.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/ggsnpicnp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gpdokjbrl.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gqsoqiqru.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gdvjhxmua.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/gmcesunbm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.tarul.cn/Article/details/gsoksuuqq.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gepgjvyrp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gkkonvnjp.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/gmxsfmwks.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gglggxkak.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/grdecjebl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gvaekacbl.sHtML

[Q25] 只取前 N 条
来源：http://3g.epnwcf.com/Article/details/gussgzedd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/ghiittpqq.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/gcpewaixo.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gvlzvmdxf.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gnjagxkns.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gxymqkzbp.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/ggfxtgtrp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gkxddwkqs.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gtandrvzn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gjysxlyxe.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/ggsxapesa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/ggxoshgqq.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gqsdavski.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gsqxyprmh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gpidqiyog.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gpifghqka.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gybnkpqio.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/ghcmjjtzc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.tarul.cn/Article/details/gwnnwpycq.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/gmesioigp.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gcimjpjwt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/ggtgxntax.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gpcwvzgha.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/glidiagof.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gqwvlaheh.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gzbqakeeq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gevlfzbem.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gehyquwkc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gmrdagiso.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gettymbip.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gwntbmxyp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gyumpcrkj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gesffnbzm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gwwgppxhv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.yfazqb.com/Article/details/gzxorgwba.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gjleybviy.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gibvebyhe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gfhurxbar.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gnrbudvgu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gmwreechq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gvgyotuzh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gzhgvzlit.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gdjoxgjnv.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/gkqsmixpd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/gbiqwhgpu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gaukngswa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fktsv.cn/Article/details/gdlbhqipm.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/grmwpedtw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gnopfdgtb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/grkvzfvip.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gifptyjbf.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/glazncvuz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gwpuotztv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/goyhqbzsr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/ghrdzldjb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gzcryejdw.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gebayfkgz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gchezygna.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gmmcfsmbz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/giqsacmpe.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gyjqyivsp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/guiksgdst.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/ghnfrxgno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gunpeghsv.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/guyhfxpqg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gfmdtgzmn.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gyrefixkn.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gnbjptufe.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gdsmwgutx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.tarul.cn/Article/details/gggajfaqv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/gnsnbkjxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gluabtzux.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gqvfozvwx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/ghkxbvtsk.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gidumxmch.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/ggvuzxgbd.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/gyiyvrnkt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gtuyuxqlg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gtkvtpafd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/gnvejsasq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gkjvorgko.sHtML


<!-- 参考信息 -->