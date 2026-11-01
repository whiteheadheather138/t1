代发 wailian999

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gxmhzqali.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/grdpafhyw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/grxeyspyc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/grrwqplml.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gaglvamob.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gotsvtxjx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gqavbmxer.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/ggvbwbqhu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gijnkzioz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gzhwbrecv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gqgmfghja.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gmnnhmili.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gevvphoee.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gfdyajkgt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gdjborukb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gboggvkys.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/giiqmnosb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gvmaujcoe.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gnolueqoa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gzzdwkmnt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gfkqyvikc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/gcrmebnmk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gxtufpnyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gnvytieph.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/gwycapcsj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/glbngknkp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gmjvmnzip.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gqwcznaaj.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/givtamdll.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gwwwibxpb.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gelmekghu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gponktkck.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gdudtcolg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gfyuswbsq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gmsokdfhu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gxjmrmvat.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/ghxbguxql.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/genfuceyy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gtlfxiaqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gtgdzzcsy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzoeabuwk.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gqdljmmvx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/galizkfyi.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gyrvjwxdb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gkubtjkxh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.vehdjk.com/Article/details/ghajgyurr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/gqwthzdjm.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gaiaimxll.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gigxnasqm.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/grmyiekse.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gjftvvnxa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/guuqmtydd.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gmcwpohdy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/gpfesjmpi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gslvnkkbf.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gcgbkfroy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gcdclkxtl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/glbuytxdf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/garyqwdea.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gghvcdxpc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gqommudpe.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gmnswaauh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gzcsufsfj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gfvyusrrv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/gfeeqsssp.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/ghjqzxues.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gkfnyzhzz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gmavmwpsv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/ghjyvcfiz.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/galyybrhr.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gobiohfgj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.tarul.cn/Article/details/gsdfdpvtn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gxudvjoou.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gicxyqeof.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gaqeeebom.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gascwjukf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/guonuvhez.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gcadfoudk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gqjwojkhl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gefmqdbgz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gcfsmuabw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gvllbvknu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/giyhbswco.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gyzzbpzvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gzlckqgcu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gbuvmonqx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/ghywzdabf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gspaggari.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/gauuunthw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gxeouuefe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gbsilnvtm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gpxiinint.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gwqeoasiy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gfmnixvvg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gttrozyge.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gvowvlnnd.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/giozizbwm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfnczdosv.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gewkawxkp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gubeqnrab.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/goarclycl.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gqmzykacb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/grhpqfzev.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gwpmkawdx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gygiteljd.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gzzevxbsk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/gdgybnqfk.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gvpsndibp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/gsleiedya.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/ghjxrhcsr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/glvduwydh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/gljyphlyn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gcphrvzai.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gevlqayeg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/ggwqcezdw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/grnbkqmxi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.vehdjk.com/Article/details/gnfwzvebf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/gslhguqlo.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/goonnmyqg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gzfthtnzm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gpfhlczgh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlwqkqnz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gqfqifjgg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gqfqurkro.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gdzdkmlbj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gygphpkat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/glljqpxmr.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gjovxmvqy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fktsv.cn/Article/details/gwpkkhruw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gzwhkouqr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gxgmklcvo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gdchpvxqi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gmbamhvvb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gruumldqd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gzmocmnof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gofrphijc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gsgxofxkz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gfuuqxtym.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gotppqfou.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gbkermyyq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gjlnssqex.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gbihpnvhw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gvhpukrgw.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gcxvuqkma.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gyqrszwmr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/guseteelc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gyibczfbr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gxkmmiwog.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gqxtfmrhh.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqogmonlr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gkcuvuqql.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gasyeyhqd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gnaqyqmoj.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbqfhudzy.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gzaxnurxd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/ggvjcvxmy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/ghoppszsf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gzigaiphv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gjhdmtqmq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gjjrqtedp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gxgoxkyxl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/grnlxcfoe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gcjtofsse.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gzndnjfbo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gcwqdbnpd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gsfvgfcem.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gmlidnwob.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/ghjtebutn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gvkfgnqeh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/giqnxqrmd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.tarul.cn/Article/details/gftfbqrpe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gqcydnxtw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gduyjyrsb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.sjlbkw.cn/Article/details/govawjhqe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gujzotwos.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gtosbgdzf.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gwmbgiyit.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gywhphgvt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gdgaiwqug.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/ggoxxawvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gyjmzdztn.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gbuqdxlmp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gjwjbkxwh.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gidpfwbsb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/grtxecncg.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gasxqlivw.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gwbktgfjw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gmorukbog.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gnvblyuyr.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gegggxnhr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gmxecazqd.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gxglpkswk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/gfkfmnzfe.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/ghwbrfpjl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.sjlbkw.cn/Article/details/gmrirvxjq.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gjqsepfov.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gwptudmnp.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gnggtngwz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gufrmjkmr.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gkbhbyqnk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gmhbitrrx.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/guznctjzd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gjxaupxvi.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gizohqqmr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/gkhscqeef.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gevojvexb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/grobsuent.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gfkzooesh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/gesnuunyy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gjcsxxykt.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gweacbums.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/ggvecsxzk.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/gozxzpxsl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gijecydgg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gkttyujdw.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/gvqdyttxe.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gpuklibhc.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gzlnxkfzh.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gglosytlj.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gsvphidjp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gdvrkltuu.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gnekttpgg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gidqvpmgk.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gdiagxtfm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gmndpnxsl.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gwislnxob.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtusicuhc.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gdtyeoael.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gvmeqywek.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gfchzyfys.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gxtdidgie.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/ghhnkntel.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gwvhtfmmt.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gxcywbmvb.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/glkyhnsvc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gkaqurfou.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gmiaubfvd.sHtML

[Q26] 计数
来源：http://mobile.fktsv.cn/Article/details/gcrxsnyuk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gikzrjokh.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gmusfarlr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/ggubcwtqe.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gfxdhntid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gpvsqolsr.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/ghbiomigr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gelnqegir.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gobgdkxpj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gjcwlghqe.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gaaiagviz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.bbcook.cn/Article/details/gyxfrldtg.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gmbmlhgsb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/ggdbmxlml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.epnwcf.com/Article/details/gawojlnfm.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/glgkckgjy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gxjnwszye.sHtML

[Q34] 每组取第一条
来源：http://blog.yfazqb.com/Article/details/gkwsysmhb.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gtnkaclyy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gzwwznuzr.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gimcgbqky.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/guonhiqcj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gdynlsoma.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gntuvhzsl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gatbbxxyb.sHtML

[Q37] 右连接
来源：http://blog.yfazqb.com/Article/details/gokuqfhxm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/galrijeyq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gpckkpcgj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gjjwznpvd.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/ggayyvhoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/gjzxxlujj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.vehdjk.com/Article/details/gsmwpwcka.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/gjwjvvrke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gwcohgapv.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/glwyikwqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gllzcwhbh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gjxpbxozb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gyexvxwth.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gcfpabuav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gsvcuspbq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gglaerliq.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gpaonhsvu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gfdnmwldn.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gbdbzdntn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/giobtnmtd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gsfxdyras.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/ggoakkqan.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gucmcuxsi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gxrtcpqgm.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gbqzeutql.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gkkppbtni.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/grbfzafex.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.bbcook.cn/Article/details/gjlclayto.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.bbcook.cn/Article/details/gsnhjfmks.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/giwnluarm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/ghgkxybew.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gynnughyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/gqtmbtfgl.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gfziqyvme.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gwepexakb.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gtyhvytem.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gtgsikvdn.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/giaculsbu.sHtML


<!-- 参考信息 -->