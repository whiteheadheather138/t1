代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gsrxqzfyf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gxhroixue.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/glzsovpzz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/giwjiwlrc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/ggygbbnpi.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gqpterpoq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/ghgtmpkol.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gmyzgcxrw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gdfjtantb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/gvsufknmz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gohzcluey.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gcwtywmlw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gxxqopxhv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gcfktbpzx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/geelhktis.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gsqmtbjms.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gslvpbaqu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gjlvnxqyd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gyxzbaads.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/goyiyhxqc.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gqtxlkiky.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gsxvazcaw.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gphhpplrz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gidewtplt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.epnwcf.com/Article/details/gahdokumu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gorfxawbm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gknajndwl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/ggvkvzvrh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/glmisczqn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gzuiwkjwl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gpuexqjad.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gzlarphce.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqxnapivt.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gstghndli.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzxxjumyh.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gvgxjyoql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gsyshuzbz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gigvxtfvx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/gqyfzhaeq.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gazyojhuu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gucaokalj.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gbbosktpl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/ghxfxgyjb.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/gtsjvuwlz.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/gyziwjfqi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gvjggofcf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.sjlbkw.cn/Article/details/gbwnszsxe.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gkkclhvkz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gjylihewu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/glqbbaaiu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gkbucdsri.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gjjxignvv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gjxwbkpsa.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gwwqtfidc.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/ghjgntler.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gwovrttdo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/gwfhbssqc.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/geysckbvj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gtvblccft.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gxpvhdjxc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gguhnzpmp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gybitdail.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gbufzjqeb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/ggkfqzcpl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gxwegbbsn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gqfeorhhs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gffgqamcq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gsafsmzlo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gpmyevkph.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gplcpdcdm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/gnmxoeagj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gvjsppzzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gberpwich.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gobkndtqm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gnizltdxb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/giigpmpxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/grznfwwdt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gjtklgsmh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/gubzopogb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhnrxgrt.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gagpdxkha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/gahcchljl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gqqsbkike.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gerizpdam.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gkmoyvtts.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gntaqlztj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gfpelmdfs.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/ggqflkmpi.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gidiyycpy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gounjsofx.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gbkajodkm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwgzbjhit.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gwimydbgf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gzfropxwv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/ggrsapitq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gjkvkcpcz.sHtML

TS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gzojhqjkf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gxlzmpevf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.vehdjk.com/Article/details/gkmjiypdv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gbvumpsvk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gzibqiohd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gfjfewent.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gneqlowae.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/gmvzeqmjt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/glrkhuhoh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gobwztyru.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/giwoxmicn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/ggbwnvauc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/gsqadbudg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gyfzasybg.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gnemiqvfa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/guubyhjyg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gdvbkypom.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/goeqtutuw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gpoypwaot.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gjzgegdoz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/ghxlgvyge.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gojlhohwh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gojuipiug.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gbjjiyxgo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/gmjdqimdm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gusqgbvwf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gemksausv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gsqfbfwfs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gcxdxgitq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gkjuyfmdf.sHtML

Ruby: x.length;  x.size
来源：http://3g.bbcook.cn/Article/details/glbjchwmb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gbdysqmtu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/guerkhhzu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gbgkqrlfw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gjihhsdfq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gmbsipjiq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/giizmzobr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gkeoykinu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gbgjmcmzg.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gqjzrvtpr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gugojuvis.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gkjcrerwq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gfzspknnk.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gwfhdidmu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gzwpmonym.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzccrmdqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gialwqlty.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gereiurqf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gfxwpkkno.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/getzbqkyl.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gzyxpwyfe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gcugycqxx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gqcwfuvpo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gliejvquy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gduelxqwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/grrjikvsb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gwhcxyxag.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gatcdgtob.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/goassrwjb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gsmgnwwqq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gdsqoikps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gdiynkkpm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gwjftxiqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gcuvvnuov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fktsv.cn/Article/details/gfessaaec.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gqzwtwhwv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/gcpoclkjz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gwnzoyrxw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grnyyhrev.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gfsxmazrj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjemozezc.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gkgonexus.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/gibdivthw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/grispagku.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/geksbkqjy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gmeaoytbu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gizkfmzup.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gxznisxgf.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gkpdwawxo.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/giojqpuun.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gwtmtqlny.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gzeipsnvn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gdevvsdwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gtazmdsqr.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gqfiidhvp.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gmxxtzgvv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gzwtvfbva.sHtML

[Q04] 修改列类型
来源：http://3g.yfazqb.com/Article/details/gryuxbute.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gfhjgdyek.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gmmhsoxib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gqruhqjke.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gzhixivfu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gsmhowwmo.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/giyskvvge.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gzpnontky.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gwtcephvg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/geyzecwrs.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gcfmruypg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/glhdplkmh.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gvbitdalx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gotbfgqfz.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gimctxfjx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gzxpaylhm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gbdjnkkct.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.tarul.cn/Article/details/gdvgyyezp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gnnwizfpp.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gthtrjbwt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/goikguvua.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/guchtsnpy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gjmocdkgn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gbuvtitkk.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gvlofybzh.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjhiwpung.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gjvmlwhvc.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/gojezvgzf.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/gxpjjbcfy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fktsv.cn/Article/details/gdeslyogm.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gtdildmcw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gmklywkmk.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gruzvixrk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gtswjgfbi.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gllrqyksx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gbhacgpso.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gixpkarmn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/gfgfgfnwn.sHtML

[Q22] 排序
来源：http://www.blog.fktsv.cn/Article/details/guygxxofk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gbckiaisp.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/gwsvbvkjj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gkegvzzax.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/gvenavtdf.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gayhwxugh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gzlesvvts.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/ghigqdgnq.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gnlgwnnlm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gzbqsbrqe.sHtML

[Q27] 条件计数
来源：http://www.share.tarul.cn/Article/details/gqmgmzqtp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/ghadzmvtq.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gpwgyhtid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gyytfntki.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gzumzjsyq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gztehjdnk.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gzkvxdhuw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gszsvqpyn.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gtwmphbls.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gyvezkksa.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gqsgaudua.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gbqoffntk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gxbfsaytc.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gecfypgks.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.tarul.cn/Article/details/gggbijwwd.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gjxxlmamk.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gnyymgqpt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/ghxfhepul.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/goejhanmp.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gspsgdpeq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/grxgpwstg.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gmzoawghh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gzjhfsotf.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/ghcdzwwme.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gvakvnnga.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.epnwcf.com/Article/details/ggvdunqut.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/geiephiyz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/gafuyvxsr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/grwspvqlb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gtugudjwd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gagspwvbn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gmxabizgv.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/ggdxebive.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gxncmijup.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gjhnzgpwj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/ggdcahzct.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gipybcqet.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/gyzjaukaw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gdqycocjv.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gaxfqihfn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gvckdieen.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gyexribub.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gddietgje.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.vehdjk.com/Article/details/gffucuccj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gtwbqckgy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gfhfkmewz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gucyodpyn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gcqbbqlgh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/ghluliuiw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gnwpnjdoy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/gjwbgvtrq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gmjgigvdv.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gfydyszga.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gwzercrya.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/glodypwtn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gbygllacs.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/glopxhlgq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gnhgkbugb.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gmzliecbl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gyyucqfni.sHtML

[Q53] 按条件删除
来源：http://3g.sjlbkw.cn/Article/details/gkzmsacds.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gdhxdayuy.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gbdnvxeru.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gffvtuwta.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gaernzaqz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gtibcglst.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.tarul.cn/Article/details/gfbhsavdh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gdqksjxuv.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gpklqnrvs.sHtML


<!-- 参考信息 -->