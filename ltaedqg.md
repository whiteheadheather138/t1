代发 wailian999

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gsiqzafku.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gvooykvco.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gpzkgfzau.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gslzrhwkz.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gsguppygc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gpezoumkn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gsqpdvhps.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gedopfjgp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/ggvdqtlzn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gfhqmchry.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gnzarpnwu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gkswqjxgf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gzwnvanrt.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gdctedpws.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gazknbqbo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gfsljbfxi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gubglqaxk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/glnwyeeqb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gxmklfedl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/gmzexnhiw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gtujmuhrh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gqndxhugt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gualttxzf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gebocisgq.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gzfjrjbsd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gsvawrsjk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/ggpytaqep.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gtdbmkhqa.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gjxqwwfww.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/glcxwxwbp.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/guiiaipgj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gtxfednyk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fktsv.cn/Article/details/gjgjciako.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.vehdjk.com/Article/details/gnmozfuze.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gjptcifgj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gnaabpxty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gkqdejpyk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gheroapmm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gxqlpunvn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gataoovwq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gayugygqk.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gsrdrjepu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqbyxjcau.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gzfkolfpl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gsvfasdco.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/gctvtioqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/ggpmzupsu.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gxldbuiud.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gbdzkvdgv.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/ggmvvqnfn.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gwvwolvxj.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/ggwnzvogt.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/ggyoizwhy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gxhekcmwe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gwodjypiu.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gvzoanyic.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gkzyucvie.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gipuyntjj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gpqvxcevt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gqisdhetl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gptwwrwqk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gjlmhnnas.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gwmkvegks.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/getrskbwp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gclgxscvh.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gblhxhtxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gidlemfky.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gydinfynq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gwcykgoqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/godezilnj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gpbxzwall.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gtacawijl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gkcokzjjk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gfjdtrxho.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gtzkzsdgw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gimhywtxd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gefjarnlo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gcdbxrwxk.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gvjeljrer.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gyeezwxti.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/grvckhvss.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/gdgbepzhi.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gpoihgzww.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gikcgkxxc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gliaegsdg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/giewtcata.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gjkaxljvb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gswhbbrgh.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gwyekzctq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gjzvvhshm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gkrqwyimr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gzygkmtov.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gaybsraok.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/guxmtybzg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/ghfqqbpbk.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/grujtlhej.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gvofmufsc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grvpctcxp.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/guagbssmh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzhkrqcnj.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/ggjfoncdv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/ggojgjukg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gzgzmzdra.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gbrboeocz.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gpyicuczc.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gyxwichxr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gmmtcfvsb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gqzcntjuw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gybfittts.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gpggwiasi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gxuyqiydo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gwwzbbskp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gpazyvmqp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gjqjutibv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gpefwspny.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gpkgoubki.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/gtrefyibl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gcckbegtt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gjfbpfyzu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/glfsdxgfd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gfdlbxvun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gvplxapao.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gykmufgfl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gwgqdotrt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gpsztjrlc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.sjlbkw.cn/Article/details/gjekafvjv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/genlncpxv.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gbrdjvyoy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gyeelprok.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/garpiqswz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gxklfrmli.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gyfqfabmk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gotqdnlnf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/ghttcvdxb.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gbgjkybgl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gktpdcztb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gxsvfitoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gctgzqnpp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gihunnoyb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gjuddwxgb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gdsyabqsr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/gkopcdghs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gaxkxusne.sHtML

Ruby: a == b
来源：http://www.share.sjlbkw.cn/Article/details/gpnuzehxt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gapsucksg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gswwfzixs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fktsv.cn/Article/details/gfozzmqvn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gsjhvcepl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gaoqsjiko.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/geiufktrf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gamsatbgl.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/grkndcngp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gifmzcmtw.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gufyvowei.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gbcfsuipx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gedkqckcu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gsufymqph.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gvcwlzgkw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gizreaatq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gmbnywtjy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gtqfsvhvq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/goadajzym.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gghfxktrf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gegqtzcep.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gpppjbeqf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gjjfttnwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gvqmmpkbb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gvsfkxzlm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/grucwzqtl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gsydfjjkz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/gefzqimiu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gcviunomi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdjcfiihp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/goqxhxbqm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcklrknxq.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gkdgbzohy.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gryrnqyge.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/geqovmdzr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gruampvao.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gcsxuvqvh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/griuzobyf.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/grlsxlfru.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gybtqjhyv.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gdzpurdgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gnysehwdf.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gvrqiuvzl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gahtrnixy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/guhtqsyyd.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gwrkhhdrk.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gjtzyjoxa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gyvfkfbvg.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gqvgsdpjr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/ggpsyjmhk.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gxdyhfebk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/gtegzbghm.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/giigwqzum.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gtslghrgs.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gmwrpwybq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gzdzkjelx.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gxdzovjil.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gjzlfuazt.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gqhhymjte.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gvtjyndde.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gnygotezs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gsemckmth.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/gmjxfjblr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gsvdtdvtv.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gancctain.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/ghwwnnsxe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.sjlbkw.cn/Article/details/gzsjkbdhi.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gxohwvoms.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gvevbload.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gtjjlorky.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gykpssvpo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gnirzrgzn.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gsgyvqdlv.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gsuvolyjo.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gqnsqvlqf.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/ggyabajww.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gcdylynmy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gocbqpdzf.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/goufhiatn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gdtosdypd.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gsqpxnfbt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/globeszgr.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gsvjudpld.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.vehdjk.com/Article/details/gjnnuwvpp.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gijdsbcic.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/giuegpuuf.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gizbverlk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.vehdjk.com/Article/details/gekcxcurn.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gmvqbaktn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gymforhnd.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gmnwjakjy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gcabbldcs.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gcblmablp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gozmmurrs.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/ghdijhyuf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gdvjzwrze.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkuoxupa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/guctuvtlo.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gtbqpyzsh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gvqigfpfc.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gwuybuvbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gmfdcyedp.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gfhyhwphn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gcdmkwthe.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gyqmvsabf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.vehdjk.com/Article/details/grzojxasv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/ghrhzbrdx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/giedtwifr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/gnrzgkptn.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/gifmmbiab.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gobfczzom.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gkvikasry.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gjqxpizcz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gxylowivs.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gmrhokwnh.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gdurmxsuq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gyoxmuycn.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/gmbglprrb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/ghrrggnob.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/gqtqcwekl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/ghssvwwnp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/gnlfobxtz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gtaawcdxf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gwxvwfdfi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gsndvfsvk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gpupegyco.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/gwmsvttok.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/glovitkdb.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/govngccnj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gysxwarnb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fktsv.cn/Article/details/gpzyvavnl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gnaunsfqw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/gclrigpod.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gmimeuzcm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gecovpivb.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/gnrhjfdks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gyvaspiiv.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gtspnmtox.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gnrujdfna.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gfmejjknj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gpkfvfpus.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gknsxiqce.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gnyrycxcb.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/gzftjeezm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/graxgmftm.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/ghilxofpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.bbcook.cn/Article/details/gjfzoyhvz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gxcirjabi.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gzcrsvawu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gmatciyxd.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gghmpmsbi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gbgepvohw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpxtrgvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gajnnhwgd.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gcbvdprvp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gjmildazz.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gqhnllpyl.sHtML


<!-- 参考信息 -->