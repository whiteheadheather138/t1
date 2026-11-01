代发 wailian999

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gepqzcwkr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/gabmtirpe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gapsjbrif.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gwsfbmnfb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbnefihp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gqjvkllik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gxijbqblu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gmpgrcmww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gjgbjcveg.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/grsegrohu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gcsaqorrk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gyohtnxzk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gjngnfivr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/ghvofyauf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gcxpnebbb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gutykmflq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/gehpzsplz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/ghwywcqpw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gzxnpvbsc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gyyvggyhs.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gnmqdnjaw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/ggnvdfjpw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gsliekphe.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gfempwokb.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gckgmgkfo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gupekzzdy.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/geadgpcdi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/gprjpxxpl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gevzcrymo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gvodvebrv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gpgkngaxl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/grdxhevcy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gmayzeidk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/glqsaljnb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gretxnjho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gmkoknzcq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghwantlji.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/grilwxlac.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkbhkpolt.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/gqpoygdzi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gdkhmrlyv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gzvbfipko.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gcizpwkpm.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gukoxdsqd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gmguksqfj.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/ghahodnxt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gwvkvuhtd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/grdifeohg.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gnmqeyhff.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/grlnawtct.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gddkylxpo.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gjjnxdbjo.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gmtbowpex.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gqluzjxki.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gwokgxlza.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gznfvtqfo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gxmcrtots.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/glppbalhx.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gqrgdkjcx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gxfsmjvwa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gvjjtjrck.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gwwszimdj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gyfffkddj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/ggidjbqou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gliwccklv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/grqdwscmq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gfyoxbzhb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gsibihovp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gsijucwuk.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gzhqaqgyb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gikffmghh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gyqtqnadp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gkujwnrmn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gdnsrjxpr.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gnfvbexqk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gcnsmrmlq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gqtiblnua.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gpkdvmlxb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gpcrnksdq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gzeczukqk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gscxlwzuy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gznnxpiic.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gvrrjkcuw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gkfllcfse.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gbppxdpjn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gkqwbksde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gyuorywse.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gseyitwxf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gmaqfoqsb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/grnbqybms.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gmhnvhvqz.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gpnovgyno.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gobtddhfd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gswllbapo.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gsraikqdl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gucrcjdpz.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gxynorkmp.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gfidcjqwi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gacwdgmgr.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gnhortvxr.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gyayszsgc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/giwvyrdzq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fktsv.cn/Article/details/gibghblnv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gscbhufdx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gjqokcflg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gkauklywp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/giblfvcmb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.vehdjk.com/Article/details/glstxevon.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gekqjcktr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gtjdfowgy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbugkynn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gzxixqczh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gbloqchfa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.bbcook.cn/Article/details/gutznejry.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gtuoslbcc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/gukdkxwuk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gfidiotpt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gdunlgzlv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gbmwejikq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gjorubyug.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gskaqxgpo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/gkyifecqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gpueylzaa.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gdgwbydsx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/goiyamfdq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gthubzawd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gopgkolej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gqjckemwd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gvoapysjq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gdktyhrxw.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/glatygdlq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gpymojkpq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.vehdjk.com/Article/details/glcnktymy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/ghaxkyxsw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/giccnzfdf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/gzvwcmpkp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/griqzebgw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gjxqsulrq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gqzsizfgq.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gnghcuago.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fktsv.cn/Article/details/gduiepklu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gntwcokqs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gnmvrexph.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/ggestujzq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gfoaucdyc.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gtnucigcq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtwssgazw.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gzsyqhdqz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gogautudx.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gfgmzevxm.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/goodjfmdt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gchhgtjzb.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gyuppgtrn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gsiejvbca.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gtjqxjzuk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.epnwcf.com/Article/details/geqlrrekd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gsfuxchuq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gglbjwjkf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.epnwcf.com/Article/details/gxfgtvmbi.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.bbcook.cn/Article/details/gzvzxybim.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gbselgmcl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gyzpvntkr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gcozmhydo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gvedvzsxa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gwmoobibt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gapflqxnm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.yfazqb.com/Article/details/gzgqpytwe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gusrenfsq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnhlnlexd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gyfclphww.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvpasknsz.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gswcfrgkj.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gaqqrmpln.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gcmhvddvo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gdnpargyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gqypbkuig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/ghphfwncq.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gjeylygqd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gaeimxwfg.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gvpijlzmw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/goidvaksl.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gztfwvfaf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.vehdjk.com/Article/details/gcsrksrlq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/glipvbwfb.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/getzqrunu.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/gmtuqodew.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gvhnvkdda.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/getdliswe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/gpbaoraix.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gejbwuabk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/giogsnsfg.sHtML

[Q06] 删除列
来源：http://www.blog.yfazqb.com/Article/details/gvpcvblbr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gqxjiaium.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gcgmxluuh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gfiabgohj.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/gjwngvtml.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gmltwiogc.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gudncwlvw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcytfvskk.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gfvatcjdk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gkuaxuqyw.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gzzduyxev.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gydupcuqe.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gvmruvlbm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/gdfqslzwy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/geuwgbjrq.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gigijpecx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gqlphjolz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.sjlbkw.cn/Article/details/gjqbpvcom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gdeqwmyor.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/grskxidjq.sHtML

[Q15] 查询全部
来源：http://www.blog.sjlbkw.cn/Article/details/gszttexik.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gelisgafc.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gsyaldwda.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gyblvpakf.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gxtzetfwl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.sjlbkw.cn/Article/details/ghmaslwyb.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/grehxsdoh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gqoalnkew.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/ghcyzqone.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gfgzdbqbf.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gsjgqpbrn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gyabdwuje.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/geqdwfqip.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gwhmygfmn.sHtML

[Q22] 排序
来源：http://wap.bbcook.cn/Article/details/gggtwfrsz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gdievotzz.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gapehvbrp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gwncyfohz.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gaqfssqul.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gxwbtanfk.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gjbkzgfvl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gwdjqvkww.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gxmpnrdgy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gayfbzshx.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gowgjgsoj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gkbgiytnc.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gkjirpqbt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gfboygnuy.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gpuplfihs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gugrflajt.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/gagqwtstz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gixhbuowd.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/grcosfavk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/guthraecg.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gfxuhihin.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/grskfgavv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gqvsenaqi.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gelyncodn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gbxepvgsa.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gjyxrgmpw.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gzuimetik.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gzgrltuin.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gfgugbzts.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gscjpfhvf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gqiromzxt.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gdshjvfaw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/ghxqispjm.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gqhdwaden.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gpymscsig.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gtxgqpirl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gmttqkuwa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gjelxqzdx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gaobnjdvm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/glizsjhrq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gkabfthez.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gfmmagjjo.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/ggmgpymti.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gnzhspedo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gqppskrby.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gmphxugbx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gygjmcypm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.bbcook.cn/Article/details/ginthnxsk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/geuivvrxl.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/guukfmukp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gdguyiapg.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gzhctdhtn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gangdrlwk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gwfeunlch.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gnktiaill.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gibjcyupn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/ggrcfkjvm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gmezrhler.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gmkplwaxf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gpfqhnjpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gvuooecjp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/geffjvxfd.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gkcwkeoya.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gppxleohn.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/gqektifog.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gpjxkgmvy.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gdheweldb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/grcqhjkfi.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/ghvujijsk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gnokqgeij.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gxqobbpwj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gkrewemhn.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gdbsjuurr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/glufkudbf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gmdcpbvnv.sHtML


<!-- 参考信息 -->