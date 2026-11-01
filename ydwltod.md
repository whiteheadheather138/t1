代发 wailian999

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gqsqsexlr.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gvkuqzwkg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gmwnkysti.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gvffevxxq.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gxoaihmip.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gvwmjbuzc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gjictuxiy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gnfycvzoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gndqytxpx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gxhzmhser.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gbsqfqhwe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gjqwhwjju.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/gwtjnqxug.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gldankjeg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gvmituaxk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gshanmgco.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gwxezzatk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gwpmzjvfp.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gamifctkc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gyjsndzap.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gjdhgrmju.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gmyfldsch.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/ggsoendaj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gcjobojkk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/giuwzpdih.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gkyqzdymg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gczvzwfew.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gywovlmfy.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gpahqqzvf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gpfyvsazh.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gmflalhnz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/grdtahvav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gmmsxxlik.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gsweosjym.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gmyqcmjsl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gdcnvsndx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gnphudsje.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/golcaqqdm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/glwylzcmn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gicelvkjv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxkcapiqc.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gbqzftucb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcyfnhama.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gvbilbpij.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gheuulbam.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/garyomvyc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gsavvgwny.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/glgcqtmaw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gkrzdttqr.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/ggejzhzda.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/ganbaphhn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gdrndduin.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gopxsxche.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gdqpcmave.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gtpptkrzk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gchxcixbu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gevaghtmy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/golgzfwbw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gzaysdaxe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gmaxitvzx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gcfylizvp.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gjflukkxz.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gkickztqu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gfplxwpci.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gkihwrpzh.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/ginshpypn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gpounhbcs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/ganfynqdn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gbobbxuer.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gvnxsegxj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/ghgewdbwa.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gtfzykfhq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gfanonicg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gmkzktsyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gwukbvncm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/guqqpflmf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/ghbdbkeyw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gdwzmqgza.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/ggzqftmqy.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/geagepxyb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/ggbwdgjuh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/grsksiesq.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gsdygsnnh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/grwkjamcs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/grtottzkk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gjgpupwat.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gtfclzieq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gwqoximbn.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/ghavxlvyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/ggtorlenn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gvlhaeypk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gugkjnygv.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gxmcpwldo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gcnsvpqxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gwcwdrxop.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gpjvpmvrk.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/glxohasmh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjizxslbh.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gqsgcevda.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grcerbent.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/ghjjloepi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gevsxeipt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gvvnjtxsx.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmkczxee.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gyhngocai.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/ghsdzsmvw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/ggzbfovuj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gamjyuhku.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gvbiyzcgq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gscfjrjdh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gybvnhkuf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gszybrhfh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gajokchhh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gcucmlquy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/ghsiycffv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/grnduimmh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gznvinurr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gusxyttxw.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gtlzsvzsc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/guudditcf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gpqxpaafg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gaycdkrqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gfsdflfyt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gtfsmojja.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/goejcpoqb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gqijkmgwh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gjvgnctcb.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/gscmrrium.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/godsehcgj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gougmtdef.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/godctwxwg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gxjppcjny.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/garznuccn.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gcbsrzkkq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gzxayjjty.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gxegukecs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/ggoihspkr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/grngoqccv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gidzfvuit.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/goilqyasf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gceynhilu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gnurqjgju.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gtjwoevcd.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gpfetjhak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/gpfvshain.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gdklsegyw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gdzsrrvll.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.tarul.cn/Article/details/gehphbzcw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/glxfhknae.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gjgpejogv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gtmsapzgy.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/gbnbrsutq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gcgmmezhy.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyvahdoua.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gjgvcztwt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/geemmjxdy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gnkmwrcsl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gokytfuya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/getbsjtbd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gkfljnkos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/grnbouulr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gigprqhfj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gwttyaqbf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/grgtmyhjd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gxiulreqq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.yfazqb.com/Article/details/gnlogemar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gprifobiw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gbbpnyboa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gkcqsozij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gcpteyzxm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gnwrvcjrd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/grcnkcdvw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gavrkfqnn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gfbdwvzrx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfpkcmwxi.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/guobqehjh.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gqzigyzmx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/guooqgdof.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gdbkkkqpk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gbiptatra.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gqklzymqb.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gcbejttux.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/guyffivyv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/giigwdxot.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gjthjdbpo.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/glaeczwlm.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/glwqkgiik.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.tarul.cn/Article/details/gytyrrqcc.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/glwmugvgw.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gwezzhwfc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gxftekwwc.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gybqfluny.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gxqjrvdgk.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gwxwwwdnl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gngorekxc.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gqihiszer.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gxkxtbwsz.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/giaiqaejx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gjyrxywut.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/giijjqhpn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/goxwukahe.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gknimpzdx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gwvuikgvv.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gpirtmysu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gklfrwbmd.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gmcbuuhri.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gbenbkuwd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gacgtpoja.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gwbunojch.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gbcrcprym.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gcthxwpor.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gxnpeebnk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gyffzcper.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/gieyyzsru.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gxlrfahrz.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/gmkzoxbvv.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gspotnhig.sHtML

[Q16] 查询指定列
来源：http://wap.vehdjk.com/Article/details/gckiljwky.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gmffvbcvz.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gwcxkgfil.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gnuavemuf.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gjoqdqzjm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/grcakxqrp.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gzvtlcvvm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.bbcook.cn/Article/details/gyuziwrwh.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gkfoziann.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/ggnvsdbyv.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gqlgsczjn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gwjjxlmfp.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gzkgmoldc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gtwtuwehd.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/gotnlryhx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gfxqediad.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gslwciukc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzginrlsr.sHtML

[Q25] 只取前 N 条
来源：http://read.share.vehdjk.com/Article/details/gdtgypksm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gptuhmglh.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/glltvblew.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjcpwdcxn.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/gayzwckaa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcktyxdux.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gxypcdxae.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gvopqqekn.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gfwofotji.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gdwrkjyse.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gpupvxpad.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gbghebrol.sHtML

[Q31] 分组后过滤
来源：http://www.blog.vehdjk.com/Article/details/gwgurkfwv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/grqokndlk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/glxaducyc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gyhbpwkop.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gxlzmpcig.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/gqyxxsoue.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.sjlbkw.cn/Article/details/gasvipwae.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/ghqjkxvej.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gawlygcfn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gmswlbskp.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gjtfbiquh.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gtytgsjfh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gzturrrqq.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/gnhdetpno.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/ggndfkvjr.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gtwiadqyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gfjieulfr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gbpytzcax.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gcbctzmva.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/gevrzksrp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gqrgcptwp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gemtjzcuf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gnxzluqdm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gbawglmgd.sHtML

[Q41] 多表连接
来源：http://www.m.share.vehdjk.com/Article/details/gualcliah.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gevknbfrq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gntfactyw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gxplfamhf.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/guskvzncz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gvopffnsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.tarul.cn/Article/details/gjelokpfz.sHtML

[Q43] 标量子查询
来源：http://baike.sjlbkw.cn/Article/details/gxfuavjbn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gwndzlbto.sHtML

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/gfrtlunuv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gyzazzhcm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gsouwgwdp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gloxeuoju.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gmvjjeyof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gvghwwhaj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gawyfinoy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gezliibgo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/gvduwrofz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/goglmquvc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/gtwwcvhlh.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gagfqvoir.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gcvejxizn.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gopntzenc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gyyaphkqc.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/gjjjamcbh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gdibesbpw.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gpbaeyauo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/golocpyrp.sHtML

[Q53] 按条件删除
来源：http://baike.bbcook.cn/Article/details/grzcfcmpk.sHtML


<!-- 参考信息 -->