代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gumykxkmz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gmnneiqcb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gqrozpryo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gfghfkgvj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gwtqzcbcr.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/gvpynzcar.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gfclyfgpk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gxbutsvlr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gqwzjbnqd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gveioadqf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/ggcrtropr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gmzdekank.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gqcdijzcc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gyqofobcl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gaoctjvxh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gseijzlij.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gnumvdwlf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gncoynhes.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/ghmhtsopy.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gprxomary.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gyijscjms.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gewtnebxy.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/ggxjrmcny.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/guuasovtn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gazhzwvyj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gmmpqqrmd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gghfbrhzf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/ghzolgbhw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gcigqcktl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gnmnqklja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gptxupglq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gyanwojum.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtayjplod.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gkbqxjxar.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gigsupcml.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/grltnwhix.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/ghsmgjrir.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gghwkjqka.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gqheffmly.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gbunhvzny.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gzjysatks.sHtML

Go:   go f()
来源：http://www.blog.tarul.cn/Article/details/gssrfrsyb.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gifsblkob.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/goigabmlb.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/gccohznpz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gwkqpphts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gwtdfzpbn.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/giwnjgeff.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gippdephd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gxwbmvvdg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/giokfamxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gkeisjihx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gtftmisqm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gviblgnxt.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gfbqvahtf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/ghzgsztob.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gtsnmoamu.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gaopprmxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gzwogudzd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gipwrifiv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gnigdgbdg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gzpryokwa.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/guktrlrls.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/giqjkwhlq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gaeazojbw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gtxlfjbdp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gotqwhteh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/grjjdmvwv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gytruwbkx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/glowtjuwa.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gpvxxccyy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gfnlyymmz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gkrxzdcec.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gomohnrka.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gjjkqbkee.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gqcucojev.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gfnngortd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gudveheni.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gmyewlrkk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/gohpzffyl.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gkyerrkin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gyzxrucwa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjvgvtkfg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/ghoxhyvpl.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gsosigswx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gghscpqab.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gupbtsbpz.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gdabmontb.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gbncposoc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpldsnhev.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gvjuurwjj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/geczwregd.sHtML

[P01] 生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gvlvusjrl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gzanyzxou.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gqicyqyyi.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gaizbojpg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gcmnzzmtq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/ghknskste.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gpvetfmlm.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gymieehnm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gsokygsju.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/gvyvojeva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gurifpdvh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/ggukxdsxu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gicwdbesj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gsxysdejj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/ghihcmvyd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gnvdbchvw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gqoxflzhr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.yfazqb.com/Article/details/glwhscmdw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/ggcexdgly.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gcdihuyxx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gfebkpndx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gjebwiquz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gtsywbjli.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gelgpykns.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gjauznrjw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.tarul.cn/Article/details/ghklbnvog.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gvnlpoyaz.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gkjdhxwgh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/ghzijqxse.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/ggzknkceo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/guuvgycwa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gojdudlha.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/geahytauz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/ghdomsbzn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gkhpnmvxz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gqskmqmxi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gkfrtllax.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gyruuerpf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gzthsudes.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/gnmxjondi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gfwrdzmil.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gyflgtlbu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gfssemmod.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gqryoncyp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/ggvppaxkw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/goyysmtcy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gcygcenrf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gnsddxvqr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fktsv.cn/Article/details/gfduenjdv.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gwrvlvmps.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gqihaiqbu.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gnjhcsltz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/grgwqndff.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gglwapvly.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/gveiouips.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gjvtkwazh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gwscycogn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gkrwblcan.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/glvhcqjka.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gdenciarq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gasdhadki.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gkziydszi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gudscngtv.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gzyssamyi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gsihodsvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/gngpcwwow.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gajlihpqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gyubbqugi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gzxfepvky.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gsaaoluaq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gjzmmuvaz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gozpysmom.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvnqizkmu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gabpamjjg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwlljaxar.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gtnjqljuu.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gmyptffow.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gyzkgoxfe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/glhstlnrq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gcbyitmtz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gmmhinufz.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gczigjwwm.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gzypywrwn.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/guducmajs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gbxkawvlk.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gdjbowhbr.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/gbsylclrb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gbfybflkk.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/ggkytdrdk.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gaxpooohe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gkkgfdyif.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gzzvbqpbg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gnxrvmjhd.sHtML

[Q05] 重命名列
来源：http://mobile.vehdjk.com/Article/details/gvckbsoit.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gxsvkppih.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gdbekkzoa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gkwzmoemm.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gndywfyuo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gefeawgqh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gyomfifnm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gdkyetxyx.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/gjzkvsrve.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnasrdjhp.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gskzflnqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gcinfpjvd.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/gbnemqpmd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.tarul.cn/Article/details/gbshmjabx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/geuhepivv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/glnbaieiv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gtgnaqdfo.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/ghoxtztqw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gbopveiwg.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/govjgqolw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/gpwugcyjw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/glwdlcwvk.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiqleuao.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/golntvdtb.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/gcjwiulks.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbhdwgeqj.sHtML

[Q17] 条件查询
来源：http://3g.fktsv.cn/Article/details/gnoqbmaaj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gmhhxjfug.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gnolajjxh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gjuylqgcr.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gdnnytlbs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/geohddyva.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/gofhdlqkb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gjtuufrlv.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/gafvyeqmm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/gzjcagted.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gubunklua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gceelsyjh.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/ghaoitvxz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.yfazqb.com/Article/details/gdoqmhlbq.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gtiksxtlm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/grwzoxydy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gfktrtong.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gkdcuqeme.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/grovzdouk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gztcuddmn.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gdschqayr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gompbmypz.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gnxwkhbxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gnfcathzi.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gakawkxdc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gyswtxqqs.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/geplhzyuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/goqqiccxf.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gqzidxakj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gmvyukaez.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gsqpfocjy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gbuhwvsvn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gkuifogru.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwxiaybl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/ggqvaprko.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gumejvazy.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/grnuinchf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/girkilpam.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gubtwjnpz.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gsnoufgdv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gdgojfzco.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/ghgfnmeqv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gasyzxjta.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gmwkkusau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/grwlzkufm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gslzzhqty.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/glskxkgfa.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gvzovyxxp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/ggkdzdgun.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gzohnzros.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.tarul.cn/Article/details/gmrentdzn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/ggcdmbcle.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gysedysoq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gwsaeztxw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gtzgelkll.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fktsv.cn/Article/details/gslxnjcgb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.yfazqb.com/Article/details/ggcsfxyxu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gyzxohweg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gyebtdnch.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/ghmddonfj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gracxsbwc.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gqwdtdmip.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gzypwndsv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gloyvyalg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gixcmzfml.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gjrliszbz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/ghlaokhbb.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gfjsdfoku.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gbznwuiwk.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gevgunhtr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gugyvcxnd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/giqmctywf.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gdqltsdop.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gdepbyorl.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gvoaeweos.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/gaxkbqpzo.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gaxuqiwac.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gcuwuomuu.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gigbnlldh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gxqbhkstr.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gxkxqcdjz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gqgqpiydr.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gmxwannkp.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gnmirferg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/ghxhuctwc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/giykyvcqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gwapqiomz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/goipuviod.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gcmhmuhmy.sHtML


<!-- 参考信息 -->