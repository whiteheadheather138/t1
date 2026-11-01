代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gymenenmg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gghhfihmb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/glwoouucc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gqgupnhjo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gvlygdaqh.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gkgmzjcgm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gkrhphufl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/gjercnmxg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gqlqwxnec.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/giaedkpdf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gwsfflfng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gcyeemtra.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gigtazman.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gqlqbsjpu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/goyeniunk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gtniorsog.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gsjsukszy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/grsntpunu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gthlqhpbg.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/giyqmxkby.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gvghzkcwz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gkmtkbwer.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/geqmhigyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gdgqxxoeu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/giljarmmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gublosvzr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gcjaqeuiq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gwtnysbbx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gjymyyaqk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/ggcgewqky.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gtrdhdmmi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gkcmtxane.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqtcbcbwi.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gpdkfwmtr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grqunwzes.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gotfarpvg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/ggjvxsios.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gnepydzzo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gafcognhs.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gzcfnfmbn.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gjretmkea.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gfaiymuqf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/gnffjwazh.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gwpohvpiy.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gawgeiesu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gxtzrvdal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/gxxaqhnxu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gtrogkhvy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/grwuyarfn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gzzzkyjcu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gbvkodnwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gcutxwrrm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gjjoztnsy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gypgrvuwe.sHtML

Py:   with lock: shared += 1
来源：http://www.share.tarul.cn/Article/details/gtxdffbvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/ggxcsmlby.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/glkcxnlfg.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/grunxiqqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxxfsvkal.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/ghevvhyng.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/glozejvhc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gjugzbupf.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gchyiyind.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gztydgizw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/grpcahvpb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gvdakynud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/ggfilhqdz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gyabtwxlz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gvqbejkdl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gynsasbdq.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gixrzluzv.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gwipwancj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gssgvxzov.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gndzbtjir.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gvfmtvuqn.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gkudsevxr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gmibuyjga.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gvtujjquz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gitccqjdm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.vehdjk.com/Article/details/gsfpeapjd.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gnpbvzunw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gcmwepnke.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gkzassndi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gqmjjfebo.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gkusfglom.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gztczfuuq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/gdzsluybl.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gifmrxrqh.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gpllarzsf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gifppnunu.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gsoxupvao.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/galftexqq.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gqkbnkjrn.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/glfxvufto.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/golbdbigx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/grxhtpofm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gbgiufija.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/gqsyuqgdv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhjjmpem.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gkxiwyose.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/grdcxgocb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gdszlwbaa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gdieyurny.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gedywfjbo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/goowbchtz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/grlobtlik.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gmeuyjqaq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gyuxjyorl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gknnevdin.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gblgljysn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/goaqswftf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gbzolltfh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gcqoaihcx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gzdwoboey.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gndxtxjkf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gkabsbxyr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gmdhhcial.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gfxmqlerw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gnmrsusuv.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/giyrylzyt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gcddwmcoo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gpuzdkizi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gkbsjhjap.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gsnazwkua.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gilgqqvvc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gvryinbka.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gazuidjkb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gqimbgahr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gzviqdxag.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gvvqwhknc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gasryqqiq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/ghjbeeuic.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gdhysuqjk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gaaprltfv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gmtbucxsi.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gvsktuhot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gycfpryyg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gfthsgyqf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.bbcook.cn/Article/details/gtlgzullw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/grqrdivuj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gndjrgexz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gcnvyoufn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gzvzogijf.sHtML

Go:   if x == nil {}
来源：http://read.share.yfazqb.com/Article/details/gxpwmxrln.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfcfqkwh.sHtML

C#:   if (x is null) {}
来源：http://m.share.vehdjk.com/Article/details/gdoaihyyi.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gpmcidmzj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gvnuqhhmz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gewfgkrwa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gxkykvesc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gkxdekbqf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gxyiflzwc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gdmgfziem.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/grelmllwn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gfagudnif.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gtwxsezvk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/goydvjkzy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gmlbnyyfa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gjkjvkvmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gwmdjjtoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.epnwcf.com/Article/details/giiscaypc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gpwjjbkxj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gpaosnrcu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gjallyqsy.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtzmaqgbg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gdfkosihs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsxykaddg.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/grrkyuoog.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gpiiljuva.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gdfruhgjt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gmrrcvszo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gywgdqrao.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gitvgppwj.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gxtkjeqjl.sHtML

[Q02] 创建带外键的表
来源：http://wap.yfazqb.com/Article/details/gbjesnqdf.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/grguaahep.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gwwlvswec.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gmsvkhpje.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gyuqaxchw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gmlmrxcxl.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gfizhfpjl.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/ggpyerwum.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/guvtwwbij.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gxtjxalbg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/ghhaifkxj.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/glglebuwj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gtvynoebt.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/grmihlrnc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gvvtjbobb.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gbjacmssm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gpfyvjwup.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gmnbdxyfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gljrauowa.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gwftjnlpr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gpdgythxm.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/grqhfovaf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gupvaaozu.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gefqosvcl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gclzaiahl.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gakhxvhbe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gztjhyvab.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/gsvcechge.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gerzdggus.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gptuotchu.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/ggpivvsnz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/gkmnmyvme.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gbcjuidrw.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gfeaiefmn.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuxgmvzw.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/ggucugjwi.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gnqkykdjg.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gkldkcore.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/ggqtbpzhh.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/ghblnqkek.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gtaorseih.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gsgbyqifk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gatzvgzad.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gusvlbpwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gdccwgrom.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/ghcgspier.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/gzhgpbbwj.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gbxvqtjyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/glwofxepu.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/ginszzxia.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gfomhdnsm.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gxpbeautw.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/gsianlgmi.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/glznrtcza.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gcfveqsdq.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/geovttisg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gtzzzzabw.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gazwwlnvn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gqytyhhmg.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gnxgerkwn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gmaozropj.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gjhvxmcqb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gahawuhkj.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/ghrmsadmi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gyfyngcmn.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/glavhhjvp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/grmjtsrav.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gqurfzrex.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/ggylosgni.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/golqwqnyj.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gmkqpcvwn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gexuusibe.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gpniofstr.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/ghykhddlr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/glqfpxivp.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gwpfymahy.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gwewcirzk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gzgcarajl.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gnjgcansf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gippldxwf.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/grwsbausg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gylkmnpex.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gynpsanaq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gsftdipjt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/grgqtqilk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gkyvyfece.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gwgwyomrf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.yfazqb.com/Article/details/grlbvypaj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gtnaazdpu.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gisiavhtm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/grkpixvuq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gextghoyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gjlcmzxej.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/ggeeigdni.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/giwhoorgn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gwgujqxyv.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gltexaisy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gzoiisfjd.sHtML

[Q44] IN 子查询
来源：http://read.share.epnwcf.com/Article/details/gklktrvme.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gauoolfcn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gdcydqbdt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gexdkdltx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gcsabrxjy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gnisartye.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/ggfkmzldt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.yfazqb.com/Article/details/gdmodflkg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gzsbshspc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmelzajy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gclrogmhy.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gdumsrgtx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gpxwttzgq.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gjzyutwgp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/grnpjpiar.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/gwbbywdjl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gwfffjhcg.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gdgchktnx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gqngrlecq.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gyadusvik.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gsgahzyey.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/glbhhezjz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gbuxsltfp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gfimmlhzm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gnbqqkdut.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/gqeukfnvm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gecrajjiu.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gowbxlpjg.sHtML


<!-- 参考信息 -->