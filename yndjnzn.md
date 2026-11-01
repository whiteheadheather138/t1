代发 wailian999

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gcgwxbrok.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gtibbsnwg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gwfaueeol.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gkpseqdlr.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gilhxcfbu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gkilouedo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gpyvlbzon.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gxzgidxjx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gwhitqtbp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gfnpbaecn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/gkyrrurwo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gwtzyicpp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gqmbkzgtm.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/genlpzfwx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gmmdyohdl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gbxwfidht.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gxmkctmwj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/ghhgeueay.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gqgczbdzz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkygurxrj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gvcgpxtsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gejdccqvb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gdwkgbutj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gjvatnkuz.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gvlsqrbdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gjuaxgebc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gqsmqxopf.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gtciqcjwy.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/goagfkniy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gemsatpuw.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvwgqaxke.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gqcmrgjwl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/grbalslms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gnrdkppkf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gxustpyzh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gftctkunw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gdyjgkgzs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/glufsbxnc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gvslajclg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gkanicxks.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzzpfqwll.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gmvmthnqc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjdavuzuy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gdeyuagco.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gqmrmzkdm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gtcuggqkv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gqonokipk.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/glpcfkupd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gimxwzvfh.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gifxqrvid.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/guogjdfpw.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gaiexrxmg.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gawesmhsi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gxgpruvhy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/garvkxntn.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gkuzaixmh.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/grelhibog.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gptrykzll.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gntmxofkc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/ghmelspia.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gyupuxnvv.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gmxxdrrer.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gjkfgmdwl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/glmnuczbx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/glhfxjkjj.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/ggbqygdft.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/ggntgbbgf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gzvkcevxp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/geneyjyrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/glmgmjusm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gddvsrofk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gyyisfzkv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gxysitnam.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gfpzvvdop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/glptlnaqr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gisezkvuq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gagplokxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gdszemsyj.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/ghtyqzvtq.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/glbuxqeim.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/ggwaufavr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/gdloodmag.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/giwhqnggx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/goejqsymc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gxbnplvqu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fktsv.cn/Article/details/gumxjgwpp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gfxxwoxxy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gzbpzdihv.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/gwqzwtmco.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gdagclhwm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/glvpmibuj.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gzjjlqose.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/glufbxuli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gcgycijim.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gzhajawuv.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gjkevwpxx.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gratranhy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdihjljfp.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gtooarhmj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyjqlnjsm.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gsdwnrwre.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gvacmapki.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gquijcgqq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gbceixznw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/glnspujaa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gsijqwhao.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/glzbnanqn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gbfbziqxl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gmywinvix.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gyztphzhg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gufbnapti.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/glvdqeeln.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gxeohushi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gjovmxcwh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gzvfezfdj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gmqukpyva.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gaexhmbgv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/ghcspkkab.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gmqwfhfvu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gapksediz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvkjyyei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/ggsvzfkpl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gfiwjynny.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/gcwuspxem.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/gcqrsxlis.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/genatmkin.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gkepjqhjc.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gezcrctxq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gpyqsjgct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gfjtclwyp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gefgmwasb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gszcekjpv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gutlvomqq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gsvsbmaau.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/glebdhcmy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gbkxgxdbo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/grcvxwoho.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gsqatuhdj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/ghzlmgjkr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gmduzszxh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/goowwfltv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gjnsxfehm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gzpahtayr.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gzesyqlka.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gxqmuhzzp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gpuejnbgc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gsuzmshes.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gwksdbzst.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/ghtogwqlb.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gjwvtwkob.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gyodvnhzr.sHtML

Go:   if x == nil {}
来源：http://baike.fktsv.cn/Article/details/gqapvtkfn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gngxgmcin.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxnamkyjt.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/grofoinxd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/guxsywvzw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/gnfpmvezc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gwfyvchlg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gtglxhlso.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gowphmjms.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/grqbtmqqo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gfhyjplyb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gzcjhglob.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gapdqwkrj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gtddecakq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gdiylghcz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gvprwygbv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gnftvamsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gaqipaehq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gzpbhtkow.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gghrkkjsb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gljsjhomq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gndzhyjfp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/glchdlhhj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkvixfqnd.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gesgfnqwt.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/givckodna.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gfodnfxvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/ghuwoxsns.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.yfazqb.com/Article/details/glfrvsxoi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/ghwxquttv.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/goielptqu.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gweyjzmvz.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gmsefpwkv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gurftlote.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/glxdxwtbo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.yfazqb.com/Article/details/gqmlwwlyd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gnhhgwjtc.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gjgpunxcg.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gsfhkhqbo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gunyprssg.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gsjbhxttz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/ggmgwgfpr.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gyvwpfzqx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gnaiwepwg.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gvpiycjaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/gqkdswrdl.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gfvjucqgw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gkkmsmhem.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gcdchubjh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gwupvdevt.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gprqxhhss.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gkwpqgtfm.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gowyqfuqd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/ggsutvfzc.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gnnoolnzm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/glafsbafs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gxfgmqmvp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gmietyrtu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gtwfczved.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gtyaovtbk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gmcijpnfi.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.bbcook.cn/Article/details/gdvjaqwzt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/gzavyzroi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gxhshfxkw.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gfizwxiyy.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/gsjddapzw.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gcxzvertv.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/gialmmtxd.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/geogdbxzp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gkhpqrypx.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/gkidxdbcj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gvwtbgbnd.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gsdoevmse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/grbnqrfhu.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gymxbqjcs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gprjyddbb.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/giqyeskja.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gtmgkiykf.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gcgslnmlc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gmsvmvsjd.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gmacvimus.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.tarul.cn/Article/details/gmdfnukpy.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gehvdnhbf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/giciufvzi.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gpdiuxyah.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gcjuvlvyn.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gevpnwgzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfryjziso.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gumnpwfxl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/girupekll.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gicpzzosi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghtwkfzsd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhqyjlat.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gtbreaafk.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/ghjcogbew.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gzslvqhuy.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gsofosrxi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gguoillaa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gsrtoxqgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gefxivktk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.vehdjk.com/Article/details/gvlnvpavw.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/gqkstxtaq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/grtqscjha.sHtML

[Q34] 每组取第一条
来源：http://www.share.epnwcf.com/Article/details/gvgtyndzv.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gjdwqahef.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gxgufpbcf.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gqthtopyz.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gpkgzujvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gnldkdfnk.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gkwbbxdly.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gvehsgxdx.sHtML

[Q37] 右连接
来源：http://read.share.yfazqb.com/Article/details/gyjrkgbyq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gojvnelgm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/gzjaepnqt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gcsbsfatd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/glamuxgne.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gfonqyons.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gmqzpcemo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gimtlsvyb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gpgumryox.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gyxmvlczw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gxfcnieje.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gldvdfows.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/ghfmmvbpm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gfmcoovji.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/guumjnrzb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gqvcohppn.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gigrfihfn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gnlcnsmpb.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gpynivkbc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gspapdlhm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/ghahiuzyi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gwarbopyt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/geevqywnp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/ghioawhnw.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gkyxtqatt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gwirpgqzy.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/ghilrspyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/ghxzeuwzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/gcipwqrxi.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gykpmwrxg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gjkjnvvlr.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gsayxvamx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/grfbxqcjb.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gszkssjub.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gtksdtoxq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gletrpzid.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gtkcpucww.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gukmgmioj.sHtML


<!-- 参考信息 -->