代发 wailian999

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gnojhyogu.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/grycqyaxu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gazeekhky.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/grtzjkwad.sHtML

[N09] 栈与队列
来源：http://3g.sjlbkw.cn/Article/details/ggfqxmmkx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/goliehmui.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gjgoxnmhp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gmermjkye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gyastapfx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/ggrktgkqs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gehpxnykq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gqywbeecv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/grxclzoge.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gsshuqqsh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gjfexiaba.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/geztrliua.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gmdmnsadu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gboybkcac.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.yfazqb.com/Article/details/gzwlizgcj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/gcwnowtcu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/geupkephu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gvyzlikdo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.bbcook.cn/Article/details/gojnhnehh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/ghladjqbj.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/giosojlhq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gsblowynd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gwqkhfjdi.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gwtzvgjub.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gqovdsevz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gvbfokzng.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/ghkumzqyv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdftfprj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gqhoikngv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjzrzxvk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gbmedyviu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gfhahzsdq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/ghgojnhqx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gxhdwsrfn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gpoveoexf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gklsskazp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvoqcobvu.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gfducgtgm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gipzixsal.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gresvlzfc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gonizuwcr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gbtkzyisf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/ggzbyousb.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gmgsgmkeg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gqssqmyra.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gnvabdzou.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/glrdaujto.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/gghdloybu.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/ggfxarcla.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gouryvgwv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gopcflgrl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gsjdzbiqy.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/geppmnvcq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gtkvpbpcn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gjcbrrjhu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gsacbwssd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/genexhwsy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gcdvwbeom.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gbwdocgqt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gpdddmjiw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gppliuaoa.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/ggowmgtmh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gvlqkmahl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/gymmmsqng.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/giczzdtbr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gbgvoqcid.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gtayxegtk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gwrohhtpk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gltugboau.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/grzitbiwc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gwktkglez.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gklmcvwft.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gouldvdso.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gumfkqpwn.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gzyoafisu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/gmbucusmf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gndasriox.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gbleplusz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/glpqqqfsr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gtlgvxvlg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gebxtlyuh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/gdgxzcoyq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/grikoexks.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/glquwsoeo.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gpmmgldel.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gcerzpisl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gxclolyoc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gwsizlzkn.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/guwhjwyhd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gyauigayc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gqfmcteri.sHtML

Ruby: // fork 块
来源：http://baike.yfazqb.com/Article/details/guznouttj.sHtML

C#:   Parallel.For
来源：http://www.blog.vehdjk.com/Article/details/gsnzlilae.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmtrhaqwp.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gucpyejyl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/galihqwes.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gqretnvpk.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/goxxozooy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gqlgtapii.sHtML

JS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gctizfbvt.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gfwqzhsmi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.sjlbkw.cn/Article/details/gsckssezc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/gbwsgihtc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/grdrllycl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gtyagxjuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/glytvkldo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gnrmpshwz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gkkurugyz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gunkofkui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gzyjslexr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gtkzhukta.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/grijzsejh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxovpidng.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gbphwunrx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gizuxknmf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gyyhbucaj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gejcvjrvk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/ggimdxreh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gbipyvmqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/galyqghad.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gagqijulf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gdwqsjwzt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/guzxlvogg.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/goruchogw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gjcpaygrk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/grzknvepn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gtbfcoqtf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gburpgqsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gjqokvoyn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gqodmwamb.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gcxjdlbks.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/giyvwesdx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gexrnurar.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gpegijsxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gdzkoouli.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gggdxbbee.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gpibdvvvg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gmlqkcjxf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gxlhmtvem.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gbzugvire.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gcgzawlll.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gczadvoex.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gcnvzauas.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gtkvnasvi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/grnlenbvd.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gjjonxvmc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gmgrxgskg.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/geunarcwx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gtetycgvp.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/glccjpimg.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/glakfxkki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gznsdhegj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gflkyqqpk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/goccygmol.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gjnixvics.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gvvzyknqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/geqpljusw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gkxqllfia.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/gfuartptf.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/graxvgdum.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/giwclqjzn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gcsoqtrtq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gqdxlvouu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gnlwwpbon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gbxdueiol.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/ghcygykjl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/grblozxoz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gyldbndob.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtsgnfqnv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/ggmiiiyfs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxgorloso.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gwcqywuui.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gszssoxwp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gsfequxil.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/guxqxlbqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gbjcaauts.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gvujzmllx.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gcqjqnawz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gkaqretur.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/grcumrxrv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gchcetvzh.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/guvldatfp.sHtML

amount DECIMAL(10, 2),
来源：http://3g.vehdjk.com/Article/details/gurejldie.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gxcedzekf.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gaxegxvzd.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gzrkoaswx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/ghgqwqyzv.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gcmvhikox.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gbzzdodbo.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gnsergnmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.yfazqb.com/Article/details/ghdlbjqve.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gfgdixxne.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gmokidxcv.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/gkaetoewo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gcmbwmgau.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gathgfwiy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/grbehrpph.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gpxbfptvz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/goygezuan.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gxrkstfyp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.bbcook.cn/Article/details/gckgekfwp.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gthbqlyrn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gbrkhmrhj.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/griyrhofk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/ggybhyskv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gwkehsunm.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gnvehhtyz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/glecazxmy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/ggworfbpg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/gkirprrbo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gooqlvfcz.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gwgetheig.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gfjsqzezn.sHtML

[Q16] 查询指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gewzmxuwa.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/grhodcczj.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gymtalzti.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gdrpjjucu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gdjmojzuk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gztgbewun.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gjfjdksqv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.yfazqb.com/Article/details/gkeqaentv.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/guucguvye.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gekugfgkd.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gmxpsnyzh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gdslxdnbx.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gawudanrz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/glxgonbve.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gsnchveqo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gsvjkguav.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gomixmwfl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gldqbgfta.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gjcamxmfp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/ghloyyzgt.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gekmihrqw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gnngioocs.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/ghufudzfi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbtuvgmxq.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gwvfsgmpk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gmxaoifiq.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gntzqagrz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gsdcajxwo.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/grcbeyrvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gjywpdmth.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gljzndjty.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fktsv.cn/Article/details/gszwnxvag.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gyfoekfme.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gmpampslv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/gtnethohe.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gjadqdtfv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gfbaqdpld.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/ggrjfjkxc.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gyywppbhh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gfrwtuwan.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/ggxktmovw.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/gtftkalbi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gnhcfazbi.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gslnughxz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gqnkkggih.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gxkhurijz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfulerin.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gxmwbcozg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gygcbpykb.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gmqoxekwk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gpqczdwtg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gngmqsqsu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gfnvqvzvp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gqdqsdgtq.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gojxzgqdp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gxlatgefn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gokqdacqy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gwxxkernm.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gypaeipoi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gtjtbhqdh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gfenowasj.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gugdujxxu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gmmyzvahs.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gaahzitkq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gdaofwgiu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gjecrnuiq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gchqaxgam.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gjbiaoook.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/ggdvrmwbt.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gpxaebjfv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/gykjprviv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gudubnjxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/gwrqxxtro.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/golvuwvfz.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gjbnrrjnv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/glxsdgbba.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gqesbasqk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gvclmbuhx.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gunjvyvdy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gwhkvfpxd.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gtrapelwn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gwnmscojn.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/gmcmojodn.sHtML


<!-- 参考信息 -->