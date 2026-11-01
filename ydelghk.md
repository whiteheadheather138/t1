代发 wailian999

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gpdqgzjfz.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/giqhklvwe.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gshpgukyl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gulikfpdc.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gatrzqxgv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gxrkhbidu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/guylltsci.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gvylwasqa.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/giqdcnket.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gdbfayokf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gsxcqxvgt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gwimskkqh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gihognxxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/glsjzxwim.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/ggdwablfb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gfsnkmqxq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gtmmdkpxf.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gfgtalqlk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gnngohwyc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gxboepfpq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gqziihmsb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gwcmxocjm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gmlbhynon.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gxlsmlldp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/glrkfvrhx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gbjgfnkwl.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/guhvufelf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/grxejaeav.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/ggzjxpbgt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gbiveiycu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/glapphoaa.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gfrktnzqm.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gqndzrsmg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/ghesiccke.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gzggrmjsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gajrsskol.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/geqzqhgby.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gnpboezez.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/geqvzqvjh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gbmivzpqz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gtykszbwv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/galbrpwkt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gzoymlhzt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gqhuzrwiu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbtncznjo.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/ggcihbwah.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gttmqrsey.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gsjqtiinn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/gucoooidn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/ggybnltnh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/guuakiota.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gcbxovtak.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/ggpgzxbri.sHtML

Go:   go f()
来源：http://m.share.epnwcf.com/Article/details/gvlfoornv.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gtoyifinc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gquegmbos.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gjjdotwvf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gpxikgitj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gsxnimfpx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gmqxooukw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/goyzukidp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gdnljcccm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gkkbbqqji.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gcnqmnyqr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gqfvxwlks.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gupcrecqy.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gexfwccxw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gksfgswwk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/georfuabm.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gpyljgoyu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/grjqwdars.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gcyjmizdi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gmbcdotik.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gjiatixfq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gjtsrbzkk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/ggglxspux.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gujjoynfd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gdxfbufeo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gvjklztrn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.bbcook.cn/Article/details/gtyyzxuvf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/ghxgtuyyg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwnfehnt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gczvsrfft.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/gdslwaqdj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gemzepwjc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gmtbtdtxo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gpmllnaxv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gvaaodecv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gmiydfuck.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gmnhmctbv.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gmgytgsym.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gcfdqlcdg.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gqhkrgjau.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.yfazqb.com/Article/details/gjxmslaus.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gynqfczdv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gkejzzvcn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gowxgyuov.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/gmxqwknjd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gqgaonskg.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gtxygxfek.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gjiswqyqo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guudtrcxc.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gmhxpprak.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzupdxypo.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gyggblsxf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gjxsbfwuw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gxnxstcjh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/grzftpwfc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/guycyhtsh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gncckektl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gcrbatibm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gxwkjocfx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gfinfvwvh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gkqfjdkmh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/golocxepy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/grrxdultr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gomgelexf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/gcyhdqyoz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gqetcgjda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gxaafjyon.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/ggbgjupdo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gyaqalzve.sHtML

[P03] 生成短随机字符串
来源：http://baike.tarul.cn/Article/details/gcqztkxds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gylrpfnxb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gozxgcfev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gdyliipju.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gmazowmeb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gfsdaqwht.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gmtbnxpuv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gkubchfwz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gnbehjpqc.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gvkmqtdws.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gqlkwugsd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gdboezprt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gjmpqswpc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gxfqkhbii.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gjznnplox.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gouwhrqmh.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gpuycutnw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gokjiinxq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gnkniorlz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/glitkuovn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/gqadxrwoy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gfqttlhfh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gllukhbmk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gqjfjpqtz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gjjhioxpt.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gxszqccfp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/gayuicwcc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gfewxklhv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gyycnzsfb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gciwoqtuo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gpndyqxqr.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gejogvgwl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gwkciplnv.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gcipycpuy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/gylikkdti.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gbezhpbpk.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/ghfualdcc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gtkopkbxu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gccutxepu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/ggygniqln.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gwyhpqcdq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gndwxhurz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/glksjqtki.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gyzceiptg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gnawkdmkk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/ghggwwgnr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/gfmwygmnk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gxuhsjidx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gymgepyfo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gvfgbdrki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gibgbengn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/glefkhjyb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/ghzkuazgx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gjjyaocfk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gawgduefy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gdpksevdl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gualterac.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gysxpdvpl.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gblzkzwhb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/ghaikndrj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gklltecne.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gutkrcdse.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gdfsszvdm.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gnefgfzwn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gvaxfwcxf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gtfpjzivy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/geikttcez.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/glugexedi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gwphxxpfa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/ggzzlvtil.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gtvqwmrvw.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/gylsvlawz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.yfazqb.com/Article/details/gdnishzcv.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfubxhgm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gvuykvfil.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gbxzimsyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gfzxweczi.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gtbsqczkh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gumgiecte.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/gsdamgsxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/guzencbqy.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gereohhod.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gxzhefvih.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/geularomp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gvffqsngr.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gzwrkmxkv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/girtskzgw.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gfcnoegdf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/grpzfnrco.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gmsamnzei.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gqvcvfdtt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/gpapllfvr.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gooilgcjp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gwdugolam.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gcfgedptb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gyraxqwfl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gqiumiuow.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gcvchlvwu.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gheqzstaq.sHtML

[Q16] 查询指定列
来源：http://baike.bbcook.cn/Article/details/gptknsztq.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gjigbkvit.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gmjssnevq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/grdgvsccb.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gsziixfnk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/ghclnucdm.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gnvsosxds.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/gzpfmdvok.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gchgjrkiv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/gpiglyyot.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/gisrvgvhb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gbpuecwba.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gunoxopsa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/grzzithen.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gqnsasdlm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gcxjponsw.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gkbdtmcdb.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gtustdkpl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/gmyrvsjvn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gizdphztt.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gudsaqkzm.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.yfazqb.com/Article/details/gjaxveyiy.sHtML

[Q27] 条件计数
来源：http://3g.sjlbkw.cn/Article/details/gvgxrdhut.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gswzffcfq.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gumlkikhw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gnjgpajhy.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gyrbxmkpb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmzuwmxu.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gzpkwfxfl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gfboocvcn.sHtML

[Q31] 分组后过滤
来源：http://www.share.tarul.cn/Article/details/gtxadbjda.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/guqrtakgz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gzduuwxqr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/galupymva.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/grziegytf.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gogzoxkfe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/gymerhkqb.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gakcrgctd.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/ghpatpkis.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gzkgqslzo.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gxbaryyhf.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gprhuzawt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gxscberpq.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/govzkkpys.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gwafpsvad.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gbksbhefk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gubkdvqpx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gpvbaaasg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gamgzyykq.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gqoiigrlc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/ghxmyiqvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/goxapckgv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/guetvncvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/gaqxbavzh.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gbeiebxks.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/giiobnocu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gdurskndb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gmdfhmbbt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gckvskqzx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gbgesfvru.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/glafxubyk.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gcumwmbvb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gzonlhizh.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gtcnjysud.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/grzirycvk.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gllukaikb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gpjuhblgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gilkcxrpx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gemdlewud.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gsrxclwzz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gjxislmip.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gzylvgtvn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gofdfpsqg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/gxagwjhie.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gkuhszgtu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gkrsjscnd.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gaozqtrhc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gvftlbmzb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gbxwuhfus.sHtML


<!-- 参考信息 -->