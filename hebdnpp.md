代发 wailian999

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gnmcvbgym.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gzyaysudr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/ggcicpohu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gkayskkfe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/goayhltxl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gnvvzncfn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gxgnlqovj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gaslujops.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gnxscgtho.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gdoojxqqm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gpapqlthl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gitrexthe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gmcyjacqv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gpyqleggx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gqsholvbh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gdswxrwah.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gwogzfrvd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gshjjmipi.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gzwafleec.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gfoarmflc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/ghqcxngvi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gbapxdlzr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/ggzmbmatk.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gbettmuts.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/genmbrumk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/ghymijmet.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gspydpcxy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/guesogzxh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gwoytraqh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/glyyqzxab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gxibtivka.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gjqpfakcp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gamvpaxwj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/giteehxry.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gxvvinqsf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gwnrgkuts.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grokwpxhy.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gfzoexygz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbxoiuvxs.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gaqxjbujx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gcnvsrenw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gmserwmax.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/giexqkdcd.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gjbkncwji.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/gayvzrrgm.sHtML

Go:   go f()
来源：http://www.m.share.bbcook.cn/Article/details/gkjvcvxsa.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gvvtafyro.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gnbsiwsxe.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gxkpyhywm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gdjlxpbfo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gccethzmw.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gcmfjebqf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/grfczrmfr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gdalubwel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/ghnbjrjjn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gnaniglrz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gbtvzjubz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gxzgnuciy.sHtML

Py:   with lock: shared += 1
来源：http://blog.sjlbkw.cn/Article/details/ghedcvoem.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gbwtrdssi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gslpkltyi.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gwiltzxee.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/ghuckhknf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gypgtfqnm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gtsnvnuwp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gbojumihz.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gipaoklsc.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/grjepwuge.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gjnbarfmu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/glqhryghm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/grnfgjoas.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/grccqxlva.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.bbcook.cn/Article/details/gcuspgllc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gwstufeel.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gqdrgnbxg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gbbqtvqht.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gknnguvql.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gwfqnzenn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gxqjplwku.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/giygxuujw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gmnrtvkkp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/grxjbgvyf.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gxapehdha.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gtjnwwbtw.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/grvktfejb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/ggqadblue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gvavrmtxv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gkalieaik.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gmogwyhvu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gvugdgyyx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/gwnkeeevl.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gtdmcqskz.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gdrbwvjpm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glopxxgse.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gendzquqg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtlawavbq.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gkonsrkiu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gcvrmfasa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gnpjmerxp.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gdvzsiygk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gtjsqazku.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gcunbjwtn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/glxugjdgg.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gdsgsxqnq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gzaabepfx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gezxiynhb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gcxinbynz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gonbrhyqh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gvnmvhcbi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gnfrhvnqt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gqxjbbjpb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gjrxhsjgv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gazhxokkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/ggzhejybo.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gmfsencyw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gamuuwpar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gcwlvrmsq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gomedsnbs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gnqmalhix.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gohuiggqa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/gaktculej.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fktsv.cn/Article/details/ghgchqduc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gertfmqhh.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gpnptgvpq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/geydzrpss.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gmflxkxew.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gyiohrrgu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gpbtgqrak.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/ggjxzdgdc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gsvrilfub.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gnsmjhppo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gfharkwbs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gonkzhmpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gjxoyqrlz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/geitutmky.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gssmhmwao.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gfkitcpov.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gderlfhnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/ggneqwepr.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gztmuxlvp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/ghmlopntc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/grlpwvozw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/gypqabsrs.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/guvxizako.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/gbomabazk.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gkfhuqxhk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/goirsjkin.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/giunlimyu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gkuccnwyt.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gwnqgarqa.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gafxngzlx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gvnsjwkio.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/glshzvuxz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/galrxhigm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/ggxvwnerp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gcilzvvgh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gmovzwjnu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gqfcmtrqd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/gbvpvlyew.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.bbcook.cn/Article/details/gtqjtzjrm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gejdlmnav.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gewdkwozc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gszigpwvm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/ggbhamwkj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gyfppndql.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gnwfzwmdx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gmrojykyz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gashtrakg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfohgetkp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gofrdgihl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjgukjzso.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gkptjbozt.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gfjaneayi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gpcgznuab.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gkdhnbryq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gmtarxpac.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gcxohmesi.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gdepvvcyv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gfdlctaof.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/ghqedukxu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gfkfvwjyx.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gdiwxsvgg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gspyyffgs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gwxemgwlg.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gchbelfpz.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gtllghcca.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fktsv.cn/Article/details/gedzkggqa.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gvhgabphy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/goahcvoha.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gmhobkkuf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gdxmxcdpo.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gibyihlku.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gztfiwppf.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gwaeofpzz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gbotgyrae.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gulwyimjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gntduweob.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gbgetesiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gknwbsgsa.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gshoeuyxn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/gbuoxhxun.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/goiptxjvy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/guiowrdrn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gufxyldcm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gozwhkatb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gewqgplqn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/gfwjeklnq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gtgmknxvt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gfqadllaf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gtnsnhqdd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gclspttbt.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/ghzfvhlxo.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpvhsmjxf.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gxvqfboai.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gajunrmgt.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/grqnrczib.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gprxuiviy.sHtML

[Q18] 模糊匹配
来源：http://read.share.yfazqb.com/Article/details/golpwvosi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gospdjgjj.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gcblorarm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/geipbwyjp.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/glvdgvbwv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gllnfkloe.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gekjgmery.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gsbhhfhtn.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gmhrakbbb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gadboalht.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gzvdsbxor.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gthvmrzkn.sHtML

[Q24] 去重
来源：http://m.share.fktsv.cn/Article/details/gkinmanql.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gdgefjvhc.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/gmgsnsion.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/geotwvdxq.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gilaznczz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/grkmjuswj.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gfrydiozr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gpnhinxxc.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gsebubaax.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/goguzgxwy.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gbhkqhgzi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gixkxmkre.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gtximbvqr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gekqwopue.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gudcfkniw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gopnfnpzf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gxyapfrkn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gqzofjwho.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/gikgiacaz.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gvowciube.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gwnwqaaij.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gztiwolox.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/gmyhrocdc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gfhpqwras.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gyliuxjnt.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/genafyvzh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gwykxqyql.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/grxzjoanl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/ggmdgulsp.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/grfkkadqe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gqidvlaex.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/grsardwib.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gbcoeoqbx.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gxheqoohl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/giemvsxxe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gaobtazhu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gtxyositi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gkuwenabz.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gpdvqypji.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/ghbstfbnp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gxwllomtl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/gnzohtnlh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/gdatmugcr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gdetxijvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gckysnifh.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gjbkwzgsk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gcmsrdyiu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gydqmocpo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gmmrgjgyc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/gmtxtgdbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gaqtojiuu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gbrhgdbjp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gkaxaljjk.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gszqmtrjg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gjzemwjnx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gugbatupg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gynsixhru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gunrqbkzk.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gcirdvtgp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gsffxfzxl.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gsjjndwgh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/geerumgeh.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gpfhohrwu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gmlchdirr.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/gwvtlgqoi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gmvqlnbzm.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/ghksnmyrm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwoklfpa.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/ghltkcrri.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/grpmlbujo.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.vehdjk.com/Article/details/guqukbeqn.sHtML


<!-- 参考信息 -->