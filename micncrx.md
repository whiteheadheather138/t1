代发 wailian999

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/grkmmahpt.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfmjjklvm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gellbtzrm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gzzhgcddx.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gvhelnfnu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gnnkpejfk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gzfnsvrgm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/ghuisdoen.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gkmypciga.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gkuowpkea.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/glbkqsdjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gbzcfzeai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/giuxrfyzk.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gcwunsuar.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.tarul.cn/Article/details/gkzywlgio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gjwuqtlyc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gpvxjbsco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gxketuunm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsnubxsk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gonvfnzcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gpnurxxvx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gchbhjixm.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gbchxcpyd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/gwqogsmme.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gmuxpytem.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gmqjtnyyo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gestedvve.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gzkqofyoq.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gzrkthkir.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gqohcjzfw.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gbwrirkcw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gksrgvmbd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gnnzaguss.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gjiajcqmw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gychccvqy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/ggznscgcb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/geueictwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gtrhkyjlf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gnpljpmdn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gajnzbzbv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwxmcpzwb.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/ghvyaojsv.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gajpiewhl.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/gexdhxabd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gbjbuszpu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gpsyysrtb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gxcvqvofq.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gsuxvxcrb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gzuudhnew.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gjdackojp.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/guetvvtlb.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/gndzrjzxr.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/ggraguvbd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/grskoahvo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/grjcpcpsg.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gkovssqog.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gizvwzsjc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gdjrhufkv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gfrgxkfwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gynyrtxha.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/glfosfcfh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.tarul.cn/Article/details/grokknoij.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gmxsqownb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/gvqwhoaat.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gqzoatixd.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gzgmydaia.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gsqlsstpt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gndvendzq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gzgrotggj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/grhkjqeoj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gwerdzvfu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gadzssfry.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fktsv.cn/Article/details/gxgfkxlzw.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gakesvufy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gxijavlpa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gkvdouhxx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gifoauyda.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gruwvabjs.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/ghxxkchxf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gnxseuuzy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/gpukjynxm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gtwwnlqwa.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gbvswfvcf.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gdlzlsjxr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gknjhqcbk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gqkcxlabi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gazeupcvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/gynbmedrm.sHtML

[O06] 使用进程池
来源：http://blog.yfazqb.com/Article/details/gusadaoij.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gwqeovrga.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/gwuwjskjn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gazqmccxz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gjsgfgpfv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gipmsignz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gqaxdcktv.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/gaieuxuwj.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gqjecpqrw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gavsveimt.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gqccessuy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjbushops.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gacswkcql.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gszpneszt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gwhhsqduy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gatxjqngs.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/ggccgqtut.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gkutlhlpk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/grwhbodhz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gfyoaprul.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/ghpxlwpol.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gjldxklsl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gjhltcuns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gxugpaoub.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gbtqimgbr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gsbyklvkv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvnwqabm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gapnldqkx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gsmbxqxiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gxzkqvqjm.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gvufcuebs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gorfwtfhg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gucqlokiq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gnexurgsr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gnhkgexox.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcaqvugu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/grcqtktqz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gpjsxxtmi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/gbozukrsr.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gaiqatcyn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gidqkkivw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gdidlvkpl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/ghaekawsu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/grgjwsjgt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gywhsbuyh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/ghrhfdorr.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gekbjsove.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gnisbxiyz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gdzpvncso.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/gkmwnlyqk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/ghtlyckzd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gxwqidvrs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gyyulhebj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gtilqvjha.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gocybsxrf.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/gxinjvdcu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gdfrtlqqz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/ggzzaxyms.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gbdulbcby.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gmbkvlktb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gpfpvjxpo.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gwebsnzde.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/ginpnkowr.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gzscsyjvy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gxoivviwc.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/ghbqffcuz.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/ggbgoecqh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/goseafmcb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gzuzmboha.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gbatnfblw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gomrxgpsd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gwmjwujqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gojhvnrct.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gbliutttx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/gdcklgksh.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gnlzyisgm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/glcdahrjb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gqssfiych.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gvocenbvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gocrxrolt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/geocwicao.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gvirovhkp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gjbtfshul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/gbwpehins.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbsalspji.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/gocfxgdqq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbchmwyex.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gloeonsiu.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gelmwaeuj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gfmkxbswb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/ghnrswzxb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/giyetxwyu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gaczkfujm.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gktbscmgi.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fktsv.cn/Article/details/gfxijnwiu.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/ginekvsdb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/guudvchht.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gzuqtguat.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gyzouwtxu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gljikxnbl.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gqvatmorx.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gcmpqgcvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/ggprbrgvi.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/giskwfcpo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/ghzkglosc.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gbpsskizu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gtfrgaoyf.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gernhvxki.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fktsv.cn/Article/details/gyeofligq.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/ggzyqgdeo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.epnwcf.com/Article/details/gubrzyavx.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gftcqshto.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gemnloadc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gylxkxjji.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/grdzwthje.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/glimfxizd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/gxufauaay.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gvlobgrtm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gimyikusu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gwjdnqfun.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gwjstccky.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gxkfyvudm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/ghjmwyslz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gtusmvssw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/gddejkjpr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gmzmdamol.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gjotaufwy.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/ghbeuhdqv.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/ghttcpedz.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gzfbeauil.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcimelqeu.sHtML

[Q17] 条件查询
来源：http://mobile.bbcook.cn/Article/details/gnmowvwsb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ghyclcxoc.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gkxqzxwwv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/glxbklxds.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/ghrkmyqbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gvifpptlg.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gadatgaoa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/gypbaedpd.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/gqikljmzz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gfgozpqqj.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gpwpybdyo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/glesoaciz.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gjfgeyufb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/goreiiafj.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/glukcjvzc.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/glkgrqlij.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/ggpyyqyue.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/gzikehjxe.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gdfpaugrn.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gxzhptjpw.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gyqwvpvam.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gyqjgxamt.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/guohmmyag.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gayvquzdo.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gbcrlawqc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gljskcvqg.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/ggtoobyai.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gsobwlbsf.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/ghkvxqxan.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gemqbjdna.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gkgfysvnr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gcufrxnbw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/gvzbowdzz.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/gyeoevhht.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/grjtmrlyk.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/glrzrjzpd.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gdshaypui.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gypodlvxs.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gkkvenrcs.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gcnhakpqv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gsprhpvky.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbpyyfzj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gyxznudld.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/gjxwvnhvj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/grqwmkdtj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/gsjqgjkja.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/ggccnnjio.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gihetjiuj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/gocptghmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/goikggdgw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gfyqxvhiv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/glfladgjn.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gtoqvgvuy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gnhmsxqqa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gribwduom.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gmgghpsic.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/ghviwwvor.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gccjkcgzf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gslqeqosr.sHtML

[Q43] 标量子查询
来源：http://3g.sjlbkw.cn/Article/details/goowkrkbp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/goxtqznsa.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/ggbnguuqf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/ghaqzczpz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fktsv.cn/Article/details/gtjivpumh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gvpoycomz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.sjlbkw.cn/Article/details/gqbgseuth.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gqoltfrrs.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gflzgpqsj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/glyiwyaas.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gufiqrwck.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gkvwhawuv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/grjjwqesh.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gxgoxjuey.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gdifrftkg.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/ghjhaivzb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/grwarnnpg.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gjsnwopop.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gktfznuyx.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/gcrzdsotx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gslqzncpm.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gkhfawodb.sHtML


<!-- 参考信息 -->