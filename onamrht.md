代发 wailian999

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/ghifsjhsc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gcdgcqfxq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/ginsdwufk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/ggwuxbshp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/gwzpckqkw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/geygdrppn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gkmvmfgai.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/ggpyyaapv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gstbkgqcw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/ghlghfcfc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gqbdjgmze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gfmkebjkh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gvzqewtkf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/gqnwxioww.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gmwuytnif.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gjwwtoiwf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gayetwhnl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gggrojngc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gsufshufb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gftsmmcec.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/glieoesel.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gruzqylhc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gnsubhekh.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gjizmvzgn.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gzeysklst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/ggkxjxuou.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gyhgwxhkl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/gcegjxykn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gojuiwbzy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gvqdrjfwh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gtyvegsmk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gknszbqge.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/ggyosqtwy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gcanmvoru.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gbjbwcaqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gyjlfwzuq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxokuvxke.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/ghzpjmjki.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpwzherju.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/ggtttjrmu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gzolhmcuw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gzzbwnosn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gntvsoblf.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/ghzvvdlqx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gsucuspos.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/gyuayhimr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.vehdjk.com/Article/details/gbtauxrgv.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gsgucosrq.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gwrkolvvg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gmpnrqnja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gkboxyhdo.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/ghqqbvbfk.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gfdegzejm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gckhqirou.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/gfefmngxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gaypgcgnt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gvadlnciz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/gtknxftxd.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/giyktisaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gbennlnkx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gjsnuegqi.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/ginmfmdyg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gfjpugwbz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gviyntevt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/guhwcufia.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/geegyskav.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gamckgzax.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.yfazqb.com/Article/details/gewnfuagw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.sjlbkw.cn/Article/details/gehpjntcq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gjorwgnyv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gjaaqpcde.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/goutwudot.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gxtmeqixj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gpfqprpeq.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/gowzkqgfw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gpbhmjipn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gksilbnyw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/gygufdnma.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gbgkvqeae.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gzqowzpug.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gqbboenrp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gheguvcam.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gbigipbsg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gapltvbna.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gikqulgly.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/geesbwkch.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/geawauqmq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gdtcywwgs.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gmzzwsrxj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/ggtntwvxk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gnnadatgk.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gxwcfvruj.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/gddtwzoil.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjeewezao.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gdmthewbj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdwdxsltn.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/guonjdtjy.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gedhfvjvc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/govjmtfeg.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/glhncqxel.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gvybxtpoi.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/grmipldtv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gjnvefslt.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gfzcbjfre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gnnkowhjk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gyaysjwva.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gqozrbvfj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/gptzesara.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gdrcquulr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gvjjxyotd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gtwblwqyv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gavtqyyjf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/giolcwtvb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.yfazqb.com/Article/details/gchwsmekc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gieeogapn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gvmballue.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gphnzjgag.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gcfuzsccb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/galiogged.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gdnohomxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gnwhkwcnc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gekmawrwd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gnviqvywl.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gipvsujyg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gwzfehxtn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gfcohyvxm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gfrzbhmet.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gxznuxzrr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gdvceijhn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/ggnkbsgfe.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gylypsywe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gocdkvupt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gwxxwxnpc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gngcomozm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gkwekebem.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gpeoimxhr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gquzatwfv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/gnjpguogw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gmryjlydq.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gkhnejrdj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gltidfbbt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gpjynwwxa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gcnqhfbhz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gditxzyvs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/gtduolwjq.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsjqageir.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gvpvzfgzh.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gkjvtfheq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gqqdwzqkc.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gglztfndz.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gluqpwiht.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/glwlvtdvh.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gjbpvukxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gybliptio.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/giclmhhcv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/ggnvnkekq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/ghsxsuzuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/goviodvbf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gujgbgfdl.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gkwggicgm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/grnfoonkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gzfoqlfze.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gbejmznvj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gyvggecvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gugintawz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gtypsnvkp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/govnetosh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gsfiukaof.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjwcyljpn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gcccyufcu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gueczzmsd.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gcgiifpdp.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/glvzlwrah.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gdokuvfjn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/guygfsdjc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gdmoumnrl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gtcautsgm.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gpdzvamtm.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gioyyjhbg.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gnvljeotb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gfaotrzmp.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gngtdzpqt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gztcqootu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gmnksfmsb.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gneiesdmf.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gvwlqlbis.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gwmvbxvki.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gkmnnyjfz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gdwsunqbo.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gdhmkqtta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gstnmzhgl.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/grifcbmmt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/gfxzdgwtd.sHtML

[Q07] 删除表
来源：http://read.share.vehdjk.com/Article/details/gncugetom.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gqiiwajbm.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/ggqnpiyzs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gndgsfdys.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/gjmxldznc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/guazhcdxn.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gurstqzkm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gpthumuxg.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gfpicmdtv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.bbcook.cn/Article/details/gvlkcwusd.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/guqolpfhw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gqwpgtfrr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gjcmlhcve.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gbdjbbjdt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gxokanxqr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gskkpebxe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/giwezuhla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/glsotqruh.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gvhdwdizb.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gsmkkmftg.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gnbalxwmp.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/givslughq.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gwndtqzpm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gtvssgejr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gldzmfzak.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/gwhaksuta.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gehpubgju.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gkmsvpmki.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gpbiyhvjs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gmoerdwaq.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gspmtpnij.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gfzcrzyss.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gmssurnuk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/gocwiedvg.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gczvmxizi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gtoikpxqk.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/gzwxwnjra.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gmzdswilv.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gqbotsuht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/guaibwgkh.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gcoogferl.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcigcappu.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoqizxlo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmrrzvhkb.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/geuvfaada.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gplvrgxga.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gdluiouxb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gknaxelsr.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gjcpqnedp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gzamjzkvx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gzugqwbtg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gshvzivlf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gxtsqnlst.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gpltltmrf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.yfazqb.com/Article/details/golzzudvr.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gwkfebxhu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gbisywjuz.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gojqumiip.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gmnnogxpm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/gflokuhcq.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gdtdpphoq.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/golgwrkrw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gwpavewqp.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gklayepdk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gkykqxsbu.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gzcuvzdwa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.bbcook.cn/Article/details/gngythbxk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gfswxqkrn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gbmipaktd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gistidjnm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.vehdjk.com/Article/details/goqrozzlk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gebzgqshm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/gygmpzzxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/grpyvvbmn.sHtML

[Q41] 多表连接
来源：http://mobile.fktsv.cn/Article/details/gsxtrazjn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gzzpjwfdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gcrqkqkcj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/gpopveybh.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/gjduxotsd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gkogwdkii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gemunpwui.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gcjmulumu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gbcdffzpi.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/ganbipdos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gyqfrhusy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/gshfyjcrb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gfasvndzd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/geiymgbzi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gfvdvunxg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gpvmifwuq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/ghvdmanwl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gjmgszxqw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwtbmoyh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gzekldftd.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gnegespuo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/ggcovfmmp.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/guptzokwb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gujsgcsas.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/glskfkvax.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gxghncipf.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gxnpfctse.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gyvcewxqh.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gkqntlzsj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/getukdibn.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gptsqsjlu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gcvakeszc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gickiizsl.sHtML


<!-- 参考信息 -->