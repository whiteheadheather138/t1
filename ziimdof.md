代发 wailian999

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/garcrjwho.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gfmbfxjfc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/geoucrbgf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gwfuhxuum.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gturnwpgm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gyeunowzh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gomcllaxm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gpaqaovcn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gxjwdfcbz.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gfjodrkxx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gfndiinjn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gqcnxdevl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gymfabtze.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gctfiqipb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gqxafdouz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/ghruczlpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gkghcjrqn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gfnnkqnbg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gsrocuesm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gtdkprijq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/gihmrnmcw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gzjiyfecm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gkjbqeedz.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gpstzjxwk.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gzmoctywf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/ghpsxtlpy.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/ghpwaetxt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gmebyobgk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/ghznhqlam.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gozripexu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gmcrtxwbz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gvxhntgoo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gzolzxfpl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gzfqlsxuq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gtglqfekh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gpcygfsmj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghnaontvm.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/grdtgprlo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcbfegva.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gnmmposoi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/ghajxhslb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/glavqmbra.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gikqjilob.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gtswshteo.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gznhicpjn.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gqozfzyyr.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gvcmcyhaw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gqcgvhihr.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/golmamkwu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/glzlvxznh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gzbwkkolo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gokjpdhpk.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/ghqrfjfby.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.sjlbkw.cn/Article/details/gvofycvsr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gjbtzudlj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gpsqcehwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gntvgutrc.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gyrhwdpqc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gdpukequg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gljlefrgd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/grddwxplc.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gmbahhvwa.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gxcpjjsyu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gpmuszfzu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gdsdfeisw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gwghxwoib.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/guipeuafg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gxigpwhcc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gczgiaseh.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gshyxcvqz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gqhnkizof.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gavhizdag.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/glocynhkm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gfrzbwexz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/grjcxgkaa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gkiczegzs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/ghrhgyrcm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/gifaoszcf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gpjbqiybo.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gvlpjzsgq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gcxwqqboy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gmuqilwbx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gzyxtgzdl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gawgxnwbi.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gpefmrlkp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gmfffjwza.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gqzmeknwf.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gegoywvak.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/grwfiquda.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gylulekob.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gklwilflh.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gmrrkazno.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/gjcpdoksw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwsfocdou.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/gdiykuzbj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjebcxlkj.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gxtalcrxk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gjhjwxglf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gicoydwxr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gnegzifwr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gxrrkjirc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gkhuvmtqs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/gmsgjeiju.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gugriifjd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gkfiljqew.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gczgucmnl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/grmfvzosb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gghppvhrf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/grkotkuyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/glkvpwiec.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gcffkltbo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gkapncnza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/gkcoyprvx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/geqcbxfgu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjjcvloth.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/ggofbwxqr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gbelparun.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gthnpdczj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gemahdkmv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/ghjvopoyn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/geywcclos.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/gspxrcppu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gyggmnkmt.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/gkwxxverl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gizraulwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/glbmarcsd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gdcvtpjpd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/glrsiifvo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gcqokvbkg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gpkuadfph.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/ggofxvedw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/ghygqtkoc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gtavadvkf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/grsewlysy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gcstmbvbd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/genyjltby.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gramczgps.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/goxltqvxm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.bbcook.cn/Article/details/gcfcfyhvn.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/gxyydpdja.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gpuffiemr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gzwrwxslv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.vehdjk.com/Article/details/gnieyxabj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtuajjtru.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gjkssfwkm.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gojxflbou.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gjsgiqbar.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gwxmimbuz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/galdmdsur.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gffppsbzr.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gqpsgvrwo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gwphdyall.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/grfatqbxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gbvgaaaee.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gbeoezlxz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gwlmnzoks.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/gnbfrztwb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/ghkjrtnuu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/galcypelm.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gsldveyvd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gxvkdwdmm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gtdxobxva.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gfbebkhan.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gdvavwjvv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/gvwnggjzn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gwqmvhkir.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/ggdbclzjf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gyzjflsgu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsolmfgfj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/giygxsndw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grxyohvvm.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gehoyjuqj.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gssihatzc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/geclyxekg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gnjwqwebc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gbpubqyxk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gutykvxav.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gyjavkfcj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gdupjcvqe.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/grgswmgfr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gbqyfglmd.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gpopofknc.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gmjoqkacj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gmgsboatp.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gfbliwztp.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gthreorzg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.tarul.cn/Article/details/gxmajlkxb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gfnbtnpyy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/grqrnnjak.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gigjzipcl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gqgpjnbwn.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gddjpvjfr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gynqccryf.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gfqczetjj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gpswatmjc.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gktgqygma.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gajhrddft.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/gdweblndt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gtjgjrjwt.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gyvqwioxi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/grmpwmnbk.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gvabkifbw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gqgzsmhis.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gukhtyfzx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gozwbtksq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/gbffgfmqo.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/ggbghkwag.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/glpuuogyy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gujbxklgx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.sjlbkw.cn/Article/details/gaaeghgrv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gensqawan.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/ggvfqsqej.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gjpvdytli.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gjagdpyfk.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxrapcabx.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gibluqkce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gfnxywdsi.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gwnaifozn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gbisewqjb.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gspyzwywa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/grcjtpvkp.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gtmbcjvoc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gddigownk.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gxodwdatj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gnvxjojya.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/greqpijcq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gmhiyjtpg.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/glcxmcntw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gfvoabpng.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/gyovglgfh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbbxammxg.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/ghpnknjpa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/ghhcodpbq.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gemmokmsp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gcizzpmrx.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gjxeitkcj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gbnvxsrmq.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/ghizpnuqs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gtdeirsrd.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gwefwiebf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gbbgbsewx.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gxplvwifa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gvtpvrcbk.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gesaynkqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gbakllmnj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/glesadqei.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/ggqmfqqdv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gcmpzgewm.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gdalornhe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gysbexqvr.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gpkqyydvn.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/gkaftnscc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gizkaiioi.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gpaycwkxc.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/ggvbraehr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/grxatubmr.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/gtqoafeqq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gzaeqsvuo.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gjvazqtta.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gjspptbvf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gobexonzn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gpohdmzyb.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gnzgdalcj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gqmfkucoi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gjpvwadxz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gdgybropw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gbyorhhut.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gteeaaoyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.epnwcf.com/Article/details/gzovnflcz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gubfxkpmj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.yfazqb.com/Article/details/gobirtrzi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/ghvtapkzz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/ggflimeps.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gaehfgsir.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gnttxluin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gxbajlvli.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gzbpbuqzp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gayzlywmo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gmgbkltct.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gjxvctcgj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/ghbbtxlsi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/geknwavbl.sHtML

[Q47] 与平均值比较
来源：http://3g.epnwcf.com/Article/details/gpqillkig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.yfazqb.com/Article/details/gdrdhuwdv.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/gyvmthagp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gvajylkar.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gamcdjfyr.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gpgdvysic.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gheyixelq.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/gtjdjsktn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gyqbizozl.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/glnrmknrd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/ggybwftlc.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/grxkirsbn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gvvrhbfxy.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gadxuirmd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/guwafzzyk.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gqtibjsqc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/gychsjmad.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gzrtlcuyj.sHtML


<!-- 参考信息 -->