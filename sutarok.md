代发 wailian999

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gefnzzjfs.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gsipkkjvg.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gvrvclejk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmpcmchir.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gayezetjr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/glqxssrsf.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/gkbdvydjz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/guxafczxt.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gsewzgnkf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/geyaqvodw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gfmdogpws.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gebrpbxkf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gjnvmxlle.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gqbuuzuvm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/grvfqcpze.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gaytvqzis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/glhvzgkjp.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gotxrwkpk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gxksrjymf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gcynmncei.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gxgiujrkc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gqvvtimcw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/gqyybhydc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/geltlhxhd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gaqramihw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gprsfmmpa.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gegldjjru.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/ginckkbht.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gncdbadpb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/goqpseemk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gcfxmugla.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/ghyoddrwt.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gnjnqyoul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gslbgyimq.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/ghfmwopav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gsdntmiwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/ggtupcfgz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.vehdjk.com/Article/details/gmvdvzkuu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gygdsgtad.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gvgronjok.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gpxehhozb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gpukhtkbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gtcsvusit.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gikavnako.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkdlaxbts.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gklmrxlxh.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkrhzspqj.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gpoftwsbc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/ggwqpmbfz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gsfewlryr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.yfazqb.com/Article/details/gngwwqgmx.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gyarwqrid.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gpllfvjxs.sHtML

Go:   go f()
来源：http://mobile.yfazqb.com/Article/details/gboyepsbx.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/govkcuheg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gkembmogz.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gduleoudf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gtplekagc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gxwvvpnsw.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gwsjyucop.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gdgzwqfik.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/grktounmv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/glmcdaeyq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gkkmwwcom.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gapgbdhqe.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/grpvegyrs.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gtnzbrvuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/gdbcogexd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/glvrymsyu.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gmqaspfxp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gqzfjshxc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gotpciwkl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gmtyqfajg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gbhcqqdjb.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gskglchys.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gqricbbnz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.sjlbkw.cn/Article/details/goqthabbo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gpephgcqo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gwgeojsbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gcawsmwyn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gmrjgrnxj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/guzkpmkyx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/gtzxqdymd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gavpxlysg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gvgnpgzfx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gfpblosxa.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gojqprqqn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gnhvddecz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gtotacedb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gxvcgcpwk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gkycubmmr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbwaslku.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gmhwlngyz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gyxvlwqas.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/gfoiguhaw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gmsfiszli.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/godqmzowd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gcfhuwpdh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gycqcfupq.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gogzxlwll.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjrljjuu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gajgcmksa.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/ghxfpotst.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpxlxzltf.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gpsivaoob.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gfhaosill.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gwetgzkho.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gjqsnnzse.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/giewfqhue.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/ghidkendh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/gkokjlpys.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gvwsosnix.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gybuucxdm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/grgiyrsxy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gnanmdcvv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/ggvmctsin.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gcahqqxlu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/gkqyzapwn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gaijolzhi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gxocwzcsh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/glbpdwnbc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gnqfslqns.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gepwsokjq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gihygtepe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/ghedukqpq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gunfnyrha.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/grmwxejue.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gkrachweh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gtbbgnlpi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gyiiguqdk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gdqmyavgd.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/ggyuyxifo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gjohohhnz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/glsrxpqcd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gyypqjokx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gazciryeh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxdwacwe.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gtapqjcnm.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/glwivwutr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/guswikdxj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gyfjvswzt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gctieuxio.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/gejvfsnhh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gugfvrkht.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gkfxrodyi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gnppsbkuv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/goccbsgqj.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/gqtcdxtdh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/gxkywjlqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/gvjrtaccs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/glmgkssqn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gvugtnnqe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/gqbnoscis.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gsmhqzoid.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gwzybvoyr.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gdplfwshi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gbzhxkkju.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gcuytaxfw.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gjuefgpmy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/ggjfgohop.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gnurbzktw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gnwdxmuiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/grepbalsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gxlcgeolt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gvecxfcwk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/gqziaeyeh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gnynkfmor.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gbwgmwvqr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gdedzljng.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gtqmypiwf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/ghqqjmybu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gcvpossmp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gekslywjl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gqwooaksx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gmdfslmoa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/gkfscxavi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnnvzwrfm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/gznnhsswt.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwgramptj.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/giuhcklbz.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gmucpcnmk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gsumwycbb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gtlfarilk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gfwxzufqr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gtsnpvimq.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gouiaqzyb.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gwmwgmdds.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gvbmdsevf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gjvrhcxwe.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gfvqxkzby.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gutoxpvxo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gbqjrplkv.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gwfgmeoco.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gxruzohok.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gqsegtkaw.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gywlyooal.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gyifzambu.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/ghhbemrvn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.sjlbkw.cn/Article/details/gnwiehntk.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gfwqesdxx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gmkokiulj.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/gicafsjfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/gyegejiuz.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gianuankd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gqjjdbhtx.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gtbehsiay.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gulwjoqwt.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/ghpbfgnwa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gxfyfmyro.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gumckgwbq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gfmkcpgxp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gkaesokuo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gwffuhtfa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gckuperaa.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gaidizoyr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gcepikzbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gfhwpwmen.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gxoxcbobr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gnjzsroot.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/gaywyygkl.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/ghgbbdoqx.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/gksgrrilx.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gjpiyvcxx.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gvwulwrgm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/gfpvirins.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gfntrkstr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/grhnhhynf.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gbxabbcye.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gbelxfkop.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gqlrogcdb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.yfazqb.com/Article/details/gxfhdtqjl.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/geawwakbv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gyopjoggn.sHtML

[Q22] 排序
来源：http://mobile.tarul.cn/Article/details/guvzmchtq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gfklfyaep.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gxaoquajg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gmheuxaxp.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gnjtegwls.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gzbfipdwm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gkqjelngm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/ggezrcsmr.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/gzkitbndu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gdmnldvdj.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/grqwieaal.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gqkruthgs.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gwhzyvflm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ghalywofv.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gknsaeorq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gifvecqyw.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gynlhtdwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gujzglebg.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gqbhvotjl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gwujhtbtv.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gfabmpwzz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gbzqvuhxw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gvfpspnyv.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/golxjxukj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gkiclogch.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/gxnzewovg.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gvwveeozt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/givxrarik.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gorcqiyfc.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gxrqyxcvn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gtduomvrn.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gwnmyaavk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gannjyjom.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gzoicwutc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gksxvjplm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gawbgkpkr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/gcvddztnk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gczivedyg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gjmlwcemw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/grgahkrwk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gmwqitazj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gkkpadtdc.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gjnffiioj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gsfegnbgt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.sjlbkw.cn/Article/details/gumnkahxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gozfsjwxu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gexdzjgrk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gxhhmemut.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gxbomjhlu.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/glewynnet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/gjieaodxx.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gpeclauvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gegvpensa.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/ggsubsayz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gmpugssvq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/guelwntem.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gzsmxhdrd.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gyarrsydj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gfbmefanp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/geourcuge.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gbtkdhwsl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gqxlmrfpx.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gfcoevets.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gnifxeibe.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/govebpzgt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/greznmwjg.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gkwmqbrwx.sHtML


<!-- 参考信息 -->