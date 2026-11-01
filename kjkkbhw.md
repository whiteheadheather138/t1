代发 wailian999

[N09] 栈与队列
来源：http://3g.yfazqb.com/Article/details/gctufgrrp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gvqauyyta.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gdpkoxzen.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/grcypnfza.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gkqmamyjq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gksvukxge.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/ggsofthxs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gecgyxrpy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/gwyfpmwig.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gffsfaqcg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gkkvsakaj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gddhdgonj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/glpviahgs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/glavzwjnx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gvsolzzxa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gquvjhivs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gurnewgyi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gvvzeaawd.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/goufftujl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gpvozvjoz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gmaagjpty.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gzhqxbtul.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gcqjjigft.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gfatdahqk.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gakdxzapp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fktsv.cn/Article/details/gcnljoyld.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gksjlcpmh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/guyumjqev.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gctobljqb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gvmmncwfl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/guhqxtvkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gsaceskwb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gcqinltpw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gwzrhphsy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/glxrhbsgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gxbrgmwgk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtrynzcki.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gglvyhbqn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giwdkwiru.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gktkiwolm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gjhcpqblz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gohdkhlzt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gbyapdpxr.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gjzetgqxj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gaozypogu.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gktvrmqzt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gzzrnjvge.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gartyshgm.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gyvhdbtuo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gzmaqbbgd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gzdqaypju.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gbjfibezq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gezzdfiaa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/grtdwyjsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyfhfenu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gnuurvrma.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gnavzxebn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gnlhmpfdq.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gvehiaytk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gsrmoafok.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsvxgkxr.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gekoagpbb.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gjrhuovnm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gzvbsxymo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gavjfalgz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gugpalcic.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gaddnfkwu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/glljghjnf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gmhtliacg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gelwcvino.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gprlrdcmh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/geevvdnle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gxkpgejgm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gimexdmom.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/ggspkyszl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gqjpecsvt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gitmfezaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gokcrckho.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gliuqqjfp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gexbfsnpj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gdpzimccc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gfmtvgqwh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/ginrtdwdi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/gldmrpiza.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gppfaakza.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/grmqyqwtx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.yfazqb.com/Article/details/gnzbrysqg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gyhvaajee.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/grxqqpcui.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgvgxqeo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/grkdwxkex.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gbjryfpqt.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/ganyvzrxr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvifkmjvp.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gzloyqfkb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqxdwhxkz.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gdtovxqgv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gwthyrbvv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gbvburdui.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gfmcjywdq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gtcjsuggr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gtfunwvcs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gldlhzugq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgiuqtxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gjirfecsx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gsidrecpg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/gyjqwwmrj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gbjxtflta.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gyahomiuv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gfhfvbwdw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gqhzxcbff.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gknszcanx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gficieioz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gatxncuma.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/giykymygh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gdyhgdwok.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/ghltfewua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/glopabqfe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/galrjjgmj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/grjugkkbd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/greoxxjuf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gqewxnucp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gswhztluc.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/gtmupnhmr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gxzgezvju.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gxowtqktx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gmrhhkhmj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gphyzzszj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/grpumdfsj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/geqrijsox.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gfnmantqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/glbwfnwlt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/grtijcmxx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/gxklrzsts.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gtnytvrch.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gduynhske.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gdqrejijc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gnzphharo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gbvscnhew.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/ggvgzepto.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/ggriyadaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gftocyakv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gpuhwuxio.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gykmmqral.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gyohnnvgu.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gbvzogwpo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gidwrqaia.sHtML

Go:   if x == nil {}
来源：http://baike.fktsv.cn/Article/details/gmvtexvwk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/ggcjnkssy.sHtML

C#:   if (x is null) {}
来源：http://www.share.vehdjk.com/Article/details/gjyuepkuk.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gxerazacx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.tarul.cn/Article/details/ghkgrakxe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gynombenz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gjzdxfaok.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gisaqaski.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/ghmflgwfs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gdjkrbbwg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gotxherhn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gpspfynvl.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/giarovhld.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gcdxgkcet.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gihaflthp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gmbafmjef.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gtqoqmpkt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/gtgsarhga.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gxhkyyawy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/ghxpheinc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/grhoviiem.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkwqajcym.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/ggqhvcqbl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmvebcrtw.sHtML

[Q01] 创建表
来源：http://read.share.yfazqb.com/Article/details/guabgrlaq.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gesxftonh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gggxwport.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/genlgjevt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/glpgtwmre.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gplbehowb.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gkhsxlrpe.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/gihnkfkkj.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/gzxegtysy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gfpyykvcq.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gwcptxdpj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/getrstcio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/glvezdpca.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gwzhnrygg.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/goqnifdhz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gwyhrzupf.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gnnhzdetn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/gwpctkxar.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/gjdcbpzlg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/ggqwqrloo.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gzfctjqyd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/goieartsu.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gtvzgqlhn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gifcdggoq.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gnjrixvuu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gsotnxcum.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gncrllcqy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gwsndgouw.sHtML

[Q10] 插入单行
来源：http://m.share.yfazqb.com/Article/details/gcpooiupw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gcybymtty.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gxnrugwva.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gjztgxees.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gqnkaxrxi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gdqyiirbn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gjsseoxos.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gzswjujpr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gzhaiohqn.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gjubajgde.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/glhbhesef.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gyvrirlhw.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/ghwdlojfj.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gdhnrkxyl.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/ggnbsdulw.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gjcfzxkoj.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gntwpabci.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gwmhbgywk.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gwliltpcn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gixiltmdi.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gfvcahwje.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/gawncdpmb.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/ghlhpdjvy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gkefoxvbz.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gezizbdep.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gcrfiirfl.sHtML

[Q22] 排序
来源：http://3g.epnwcf.com/Article/details/gbdnevblj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gulnmmalh.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gpqhkmzeu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/grzbqcfnq.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/guvanykgd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gcomkhgnx.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/gbkdixlei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/grdmojpdn.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gjaawifyn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gxxfsjeuz.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/gayecsygb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gkbiqktfk.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gelezncob.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gjogkzrsx.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gbxhbslov.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gmtpdnvxi.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gpxzvyzan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gakdxludn.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/gxgxioixl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/garuagpsb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gknbqnvww.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gdgdtkbtx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gfaxnfwwi.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gvwitwsld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gedoymjpa.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gpttohrqi.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gluvvtxjp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gmiasisip.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/glpfypmye.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/ggzgejycu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gceyvxsmz.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gdawzqliq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gcsqlgqiu.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gebmckqlr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gvcjrcbfi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gqyoxnwuy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/glgizsxbm.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gnsnlmegl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gsirursye.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gtdcojxeo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gxdqqreye.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gbhcjmcfm.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gjdsmhzbs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gtcphmxbn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gobehulhi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/goytovppm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.vehdjk.com/Article/details/glpbrgsrl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/geffyjrfw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gdslyolud.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gdgwqetob.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gvechselh.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gmpuqbxhm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gzpbpbhvn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gkkmvcwmy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gznbucyof.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gubmifzka.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/ggoatzqre.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/ghmyqkknk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gxcwdmehy.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gdgzaywot.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/gatbmgkvz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.bbcook.cn/Article/details/gxxbjqlte.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/gbyvkojbe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gadnpxocn.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gadyloadl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.bbcook.cn/Article/details/gdcxbiqvk.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gytbscsqn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gjcshcxvo.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gzswdhtqv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gtnfxxkvd.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gkstdydnx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fktsv.cn/Article/details/gdgmgfjrd.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gwldowcnw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gaaphfewo.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gwxvpddsn.sHtML


<!-- 参考信息 -->