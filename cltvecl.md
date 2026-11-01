代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/gktmvlbxk.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gwbekvnpo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/girucommj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gquvfrkuv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gplfrhoxy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gcbkpvjgl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gldjzsewg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gwrfrwzss.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/grprkwrcv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gtnnwyyrh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gcpisriyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gplrkcgpu.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gqmwrxnqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gqdlobteb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gdjpjjaec.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/glcjrizrg.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gkybhkmqe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gmgqbpyiu.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gilpvfwbs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gkgtifrou.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gkavnzoju.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gyubzmtis.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gowbyikuq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gztayemdh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gfdrbevyl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gkqpripbm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gldxwcuvf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gudktnche.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzxdvecqz.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/gltwdgjlt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzvnqrexe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/grrmlukxa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gmxrgalin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/giyigzjtm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gbquvtitz.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gxaxhfldd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gyglubxkp.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/glwdnbaaq.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gyegivhnb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gaxkhjqlk.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gftnmfkem.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gvaawzuoo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.sjlbkw.cn/Article/details/gzabticyb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gqyqbnhjt.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gacbiblij.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/gqivwxari.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/ghwqpxhms.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gwtxhpsui.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/ggdvduasm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/gtzvsyxqs.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gnkhaquvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gagosskux.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gpezdlijm.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gekutsjje.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/ggnyevkil.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gyvvqrtmn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gbcagdeel.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/geigqkfkb.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/giquyaiku.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/ggqapvdvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gwgorczld.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gknlqkgcq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gnznbfasj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/grmfoalyd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gnjceivzx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gomfelnjw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gfevlhjfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gpqmcvivt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/gmpeobkyi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/ggmbawtck.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gbbxbjbod.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/giqhawsxf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gpthjfmpi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gpsddggad.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gmqtmxbez.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gwkitmifn.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkeqagpj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gasppxzsc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gckdopstv.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gucdndngf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gxxkdijrh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gdadwhhon.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gmeckprag.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/ggdwzifph.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/grnoklvse.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gipfmszpi.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gdphcawdg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gweekzhla.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gspsegdop.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gmvpowpbn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gyawhtrjb.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gbmkuftlz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gxgmunizk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gmmiyttgh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gzikdalvu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/ggqayfggm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gjhfznddd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.tarul.cn/Article/details/geonnblnd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/ggyccypuz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gypeldwzi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gzicwnbfr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gfhvtuwpq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/geyrshael.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gztwkncmb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.vehdjk.com/Article/details/ggdtkiqqt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/ghsxuvhhs.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gpnodxwyi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gbtpasixy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gomdogksy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gyrjxsnlb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gdpckwhfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/gzjvnsgpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.sjlbkw.cn/Article/details/gwcjtmowl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gttagvnfp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gqclcitoi.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gevtsbwjd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gifmvidja.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gwljppejm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gbrbuiszq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gvrmvzukc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gxnluqnmv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gqyrnsgot.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gdrubyvid.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gxmvonpzf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gguguohpt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gtjxcnbpw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/gaempdctr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.tarul.cn/Article/details/gisfozfia.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gkvlgijig.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gppdkmahm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gnegepmle.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gknngoqhr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/gzoliavms.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gvpincmbt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.tarul.cn/Article/details/gclohlszn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gaccikjrg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gkeblsofy.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/gyoygwhzy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gokbcfkqh.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gkfvhwpyy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gcygvxwis.sHtML

C#:   if (x is null) {}
来源：http://m.share.vehdjk.com/Article/details/gururigcf.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gvlxzsjmq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gpontzbmp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/galkrohya.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gjmvqswqs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/ggxktigme.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gtrrszrzz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gwfcpblej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gvxiorygo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/ggzvqmavl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/gvmijrymh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/goujqdebo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gyowhwzya.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gysqhsotl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gkxqbbwtg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gcuruzoew.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gntkxrmcn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gjyzfwgkh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/grlqlgzms.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggmrxvxzv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gbexwaspc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gruycfwoj.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gvmwzkfta.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gdhacpybx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gkssqxhjd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/goxtemsvh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gjxnddvsw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gqrociptq.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gqfzxzvcs.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gnpaezudf.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/gupktbjkr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gptcpmjxd.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gcmpvfsun.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gbtdyvfss.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/gagiumcdm.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/ggaeuqpnx.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/glzmjitjd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gzejweyfi.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gqtygiaci.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gjjfbdvif.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gohjwgjlz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gaeyxsfmt.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gmoieremt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gmtiaqlqr.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/garlgkeyh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gzsqawaxl.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gdluszilj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gytxuhcyp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/gvfzosczp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/givwddlve.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gkzvivrhv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gtxknbhdt.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/gmbuwaxnc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gakmuohyv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gocfjokjh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/ghqxbfqen.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gmomienjt.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gjsecxuwt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gkycwemcz.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gbobulavb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gigyykdzm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gxcphotpb.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/grezbaqvj.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/ghtxesnvy.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/grvvbfpgu.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gmirzjail.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/grvhnqlbv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gfiqtgdys.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gmpkyocbs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/geugikimf.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/grqfwuytp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gfmkivxag.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gshddycmk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gbvaafewf.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gogdbogil.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gvvcurhia.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gyesqyjpy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gglsnsggm.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gmxzwrlnl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gnljayqyr.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gwgkvuhdr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gmqwzjywd.sHtML

[Q25] 只取前 N 条
来源：http://baike.epnwcf.com/Article/details/gxhyhsmba.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gmmurufpt.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gjshsdcta.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gbskxzdoj.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gfuvdqlgu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/giebcuzru.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/ghfnoowgr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gqwtswcgp.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gyrswbjbr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gcfmsixbg.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gkdkhhsux.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gjoylkwgw.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gbnpeurht.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gditfyfgp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gulejaidh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gpuzidqfe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.yfazqb.com/Article/details/gjttdtpqo.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gktfmynnx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.tarul.cn/Article/details/ghefacmri.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gdjhggqeq.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gnmvxfivs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/gwpsetlmv.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gnifwxema.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gcafnolut.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gqsboyxyl.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gkcwkhhrz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gybxgbpec.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gczypaybd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gpmavwnxz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/giihtrkiq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gpxajgzwe.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/grnlqgknc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gczigzgxu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fktsv.cn/Article/details/gtrriokyz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gnctobbqi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gvlkbijcy.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gtdvdjcft.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gihmnehwo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gxnygzfsu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/grlhqwbde.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gqiwnzbqx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gulifmkzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gbfdsycfm.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/gopibgada.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/glqekzucg.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gdglckqwd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gayirjwvk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gtbspnyas.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gvrmmizqt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gqnvhcatq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gkrsajrec.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/geiajhbki.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gopmmtzmp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gtzjtdcqv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/gejvtmvii.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gzmifscfb.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/gddgsfzau.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gvucsejjw.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gsoujetcy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gmohglmxf.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gklquibqh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/gmaxxqktn.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gigirfpnn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gvxihdagn.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gsskldqwb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gsgmiipej.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gzwimvupg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gdpntlsqa.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.bbcook.cn/Article/details/govqvwltv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gmwhfioic.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/grhyazdzm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gidtranty.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gitwqxjmt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gkagquyhm.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlizrvks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.yfazqb.com/Article/details/grdqphvmg.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/glrfvalih.sHtML


<!-- 参考信息 -->