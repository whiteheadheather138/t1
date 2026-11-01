代发 wailian999

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/guwffrjxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/giwiwuhkf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gtadmrkcl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gzrgofwua.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gbhdmmklv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/ghebkbkts.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gawvbznye.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gbbntcapn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/genphhezr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsfbgsvz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gnexspqgp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gqpzewhzb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/gwgtuajjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gdcireolt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gcqttkcsm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gdxtbvpfj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gknrnnaeg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gisemmnze.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gmashgizu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gbvyiucgi.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/graewyovp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gzbtshtoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/guztfzuur.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gryknzwhu.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gpygweoqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gzfygvfnq.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gfumtxsjn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gaelgdhhd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gmqaltuyb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gzgnffmbs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gyqppvfrs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gbiyisbsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gzfidvkxr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/gumutochz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkdggkpan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gupmylybb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gckvjrfye.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/ggwpksitm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzzyqgefu.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gybzrvlbb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gslhhcxnj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/grndendxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gwgdfdocc.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gvuihepjr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gqcptlokc.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gmmexaipr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gkrmlscfg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gltlxhcia.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gtqzrigvm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/gieyrxsnt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gcepipbeo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gpxzxzxsz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gqicmksix.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gjszigjeg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gyvqzzymf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gwgmztyea.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/grrqvehvl.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gdctkzqyx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/guopcwvch.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gitlefcus.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gzbrtwxep.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/ggacnqvnl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/geydvffpj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/glpeuvkyk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gfecsolko.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gfkrynjpa.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gdiqdosdt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gpuihmihy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gdvmpufqo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/goesgtiwn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gkqwhrkwa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/guwlqyptu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/gdzywedkr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gzgtesrxi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gbbtoazqn.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/grboawawf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.sjlbkw.cn/Article/details/geiosleif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gjugwvzzi.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gpfqryrrv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gmduvcqkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gcyhjqmix.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gqauokytq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gpdghzubp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gdhvavlmz.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/gzkvhchap.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/ggmwqhwiv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gdidpodve.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/glbdgfvgh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gibivlrju.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gpmhjzvyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gtgsakdsg.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gcbnwmopk.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gcinawckl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gunminyrb.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/grpaijkcz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnxzvaqlv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gubchdhea.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/glgrnctjx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gojriobvp.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gseqqckre.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gphiqlwta.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/ggiefquef.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gsujjydub.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gusqmugvw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gjurbvley.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gcihewkpq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/grmmkhtil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gbbjglcjc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gbafsrnko.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gkoralrsa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gewyavqrz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gljybhnje.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/grvdatdyu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/giqfjvdvs.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gmavqqvcx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/gtuvpiqgn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/ghzalgbnv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gcaxmkpsa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghmjtbzdw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/gueoznmua.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/guqaomofc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gcpnehbiu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/ggzdfmrsn.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/gofuqfmbr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/ggvetgzbr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gcriaqhev.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gaueoquzk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/ghezwapfu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/ggnalgfco.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gnjjfmvuc.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/goqqmisii.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.epnwcf.com/Article/details/gmkcmbayb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gqshfkrln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/ghzeaxxbc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gblyuyibs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gxsyedsza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gmknwiydl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gjyidfnnu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gbtkzbwac.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/guvzxxhfk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/ghqlurbqv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gaptasntu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.bbcook.cn/Article/details/giycxokzz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/glgtqydlw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gymnldrkg.sHtML

TS:   if (x == null) {}
来源：http://read.share.yfazqb.com/Article/details/gcdewuuac.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gellfseiw.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gfskdebmt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gqmkwbazi.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/ghhimwley.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gcktdgfhb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gjvtptrax.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/glddixyti.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gbcmcsddr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gwybrbfsa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gbqlgeuno.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gpccjvnwj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gwjjwuwzz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gqdtmzwcr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/gvhufwkes.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gnbbjhcax.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/ggwhgkzoy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gqoelhzyo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gpeqiuaxb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gmieufetj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gwmqpzmmy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gypuxkhjw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gfycirncw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/guwrjntux.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gxyxntxnn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkypbybdq.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gopcjnjix.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/glngdfnam.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gdqdoshcj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gahscrajs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/gsalixopp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gekhvuqux.sHtML

);
来源：http://www.share.tarul.cn/Article/details/ghlvjfozk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gheljruln.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/goqedohzs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gvfdkohsa.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gnvvsgmqs.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gnrefeiad.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhpjfhyo.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gubkdpkfl.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gestaifmf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/goihpupsc.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gtktkcdde.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gndonkczo.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gxrfjrrxa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gzrgqvpul.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gujajlzpf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/gqwqlryqx.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gchhkrcgq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/goertzmqc.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gxayovxir.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gtmpzipvo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gpjqxywzj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gwqgjfrur.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gnisxodtk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gihinidgd.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/gfrmtebox.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/ghigstujf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.tarul.cn/Article/details/gtjidcghk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/ghduderni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gztehmvqj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gnjgrapaw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gfowsxorx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gamdgbvoi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gjngxhybw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gyoebkbge.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gxrdvosde.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gnlsjhawv.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gqylwhosd.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/ghdzbkrev.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/grqxhkslv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gaqvjfogw.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gvbnvkpvh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/geizkhqtg.sHtML

[Q19] 范围查询
来源：http://wap.tarul.cn/Article/details/gcvfjzdwc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gzqlftazs.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gqrwydhig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gjnvzovsi.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/gixwfoasv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gvxubmwpy.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbrnguzr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gnjbkbkhy.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/ggkwgufky.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gbjvbuvna.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gyabgqgmi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gfvtbdsnx.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gbuafumko.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gxgwxvbeh.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gfaulwhyo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gtixyzlhb.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gybezyyud.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gghadsinw.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gmzjppwat.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gqvlaqtjx.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gztpvrmuz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gpsiodhuw.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gvsjikibf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gitlvudzt.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gdqmovxpm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/gxcmwyhfj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gxalowpww.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gdoijahhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/glsidzgwf.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gwevpvowj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gpgxkjywz.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gatxkfweb.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/gezsumqiu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gbntnsnko.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gpqplqujk.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gtxgerpkz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gwqptmlzz.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/ggpphfhpx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gupyqspmt.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gdnqdpihb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gydizeygz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gajqjpmos.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gnefytnrm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/glulfvyha.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gcyellsmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gmsjvplww.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gegevcjpo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/gpuaszztb.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gnsmbrtxa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/gznwgwiro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/ggqliajzy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gtxjxcaoj.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gyutezeic.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/geudetnaj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gfgtwxrio.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gtmjibmaa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/girilmlxp.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/guvcdeaqe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gjwdvxrqp.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gmbdwhhll.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/grdrfbolb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gjxjbednp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gqorqlxcv.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gprcdbynk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fktsv.cn/Article/details/gyshtcadz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gmcekyzqu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gqofdnyva.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gwywqhgdw.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gctbqvlcl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/guuzfoyvs.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/grpxyqdvm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gtwnuynyn.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gsgwlbquu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.bbcook.cn/Article/details/grdkiymix.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gzjwepktp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gnuapyvrb.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gydzcljnr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.yfazqb.com/Article/details/gjhkxcexd.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gjchqskut.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gitohswkz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.tarul.cn/Article/details/giqgnztsn.sHtML


<!-- 参考信息 -->