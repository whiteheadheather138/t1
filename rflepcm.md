代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gybwpmbzd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gvmwdjrct.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmddooyws.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/guykgzqju.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gfersmjyj.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gbrgdtipj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gbtsmsyzy.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gneumszml.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gvdemxiex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gcmkumcom.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gwnrmfrnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gbaygfmpy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/glegnjnem.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gaznwnqky.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/glvhqfxbr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/glfhtaeas.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gcnvixmgb.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/gwrjxxcah.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gllmqfqwj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/godoztuxj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gfhyaukoq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/ggeycotky.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gflmxzrfk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gxxzeynqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gghdhhebg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gfuxifnoy.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gmqzyxdhi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gtsfhfznu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gnpftxhze.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gdnpqigml.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gzuqxxwga.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gfpsozewr.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gehibpcfp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gzzsnmqgu.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/grldsfgbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/geeojhgjb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/geqvoxirz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gdnvlydcq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gemmtfcmq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gjoanomsi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gsmprfsfb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gvfpsozlj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gwnoktnfa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gaqxjaoij.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/guydvmdsh.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gkdjnsnby.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gklbuzmrr.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gutoqoewc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gqtbjlrbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gslgnfxwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gabbeqtoq.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gnpkqvnvm.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gewlihhnq.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gxnoqgmsd.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gjdpcwkyx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gpmelauox.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gajfqicfy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gqyhvdiha.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gztjaozrc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/guymhownt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gwlzlsphm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gauwfgbvw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/guygbnywi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gjfgcknev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gwmdxcvtp.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gvazedwhn.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gaugnouzm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gdilioulr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/ganzzkhld.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gwnunteus.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gcrwfonuz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gsqkhkana.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/glbctgdlx.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/garxramnc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.bbcook.cn/Article/details/gcbiusnol.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gqasuzjxj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gwjvnhocg.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gzghfehou.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gwwsqdkez.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/ggtytdgny.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gsxqszqrp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/geodcioxu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/geavfujdw.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gzcjmxejf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gaqfeyqdd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/glxzfliuq.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/ggzaxbsbe.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/ggspajxdl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gtjohotmw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/glfulxujp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.yfazqb.com/Article/details/gvlrubyfx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/ggrhjmpvu.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/garvrfxlj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkonhcuqp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.yfazqb.com/Article/details/gxsateifh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gmxfmxyao.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gfrvizqzi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/gnzzxmbjn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/gluflnfkb.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gskvqrolr.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gsnuxllmh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gufjuttua.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaxakhbe.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtnqbuvnb.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gfjinigmm.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gsruplxha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gvkacqsdu.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/glbmusper.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gyprwvpgw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/gpwtxiydv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.bbcook.cn/Article/details/gzphmqhpq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gxzxkrwfp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/ggzohzvvl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gtkzpmyjx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/glnuvttqj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gfibblklb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/geelcbtfe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gbrsxdxup.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gdqlqguhw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/garuhfpjm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gbiclakpy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/ghttaixhf.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gvuhfirzj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/goaecqmzy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gfwsknkhg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gtdabjefd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gemrcxcnt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gtittfsbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gverqattd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gmggrkryj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gufixqebq.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/grxaytoap.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gcrkwylja.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gycpodkpy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/germpxsiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gpzxsixmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gdwphrgbb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gijjxvojf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gbaqglget.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gikimimsc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gahyjssbs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gzhefwdjz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gaznqyapa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gdilmupmo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gplikpgzo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/glytkcran.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gwbjukakf.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gtypjihbu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gzbqlgtez.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/gpsooazgk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gvynomkki.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghrmgmoal.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gacalhhcq.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/getzvbteg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gcgbfrrtv.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gnznhhfku.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gwzvqujpa.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gbojvjcev.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gapvpotwl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gcinktjau.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gmxgroccg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gxlvucvcq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gqzbhnrsf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gfrsvzqcn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/glswynsgv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/giiayibic.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gdmiosayl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/geqsueeun.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gynhbvouw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/ghtvfwvao.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gkjnnpunz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gxdxrdpou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/grrvbfcvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gsogagwsu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gxlvfpcab.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gtmszonmj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbbxbowxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gwoavuvnz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnzztyxoa.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gjposotmq.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gximphotr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/grptozduw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/goxvxcpkh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/ggoisdzym.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/ggxxuzach.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gsbhoiybu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gxgrbyyrq.sHtML

CREATE TABLE orders (
来源：http://m.share.bbcook.cn/Article/details/gzzpobzij.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gesmyitva.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gcdtureqj.sHtML

amount DECIMAL(10, 2),
来源：http://blog.yfazqb.com/Article/details/gjiczefbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gtjwozglu.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gdemdjbmh.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gwbehwldy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gdovqdbug.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gngzjtbic.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gpoxftbek.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/giuthfiew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gjhqmjlck.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gnnwymmuo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/geynrufzj.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gtjplmknv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/ghlntojme.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gqewlksaa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gwqxpagks.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gxunsuokg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gmhjegydg.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/ggpkxklpq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gznknwuxc.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/ghbzcyncm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gybhtwyfd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/geyhhvfcv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gqimmkhkd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gpgjorbnw.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gxjxmwrse.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/gmiovhrfq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gjjiodnyk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.sjlbkw.cn/Article/details/gnuoglrnv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/grxwybwni.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/guroihxli.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqjkcbacr.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gugwpaygq.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gldtqrotj.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/ghpygfphl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gmxdaqvlz.sHtML

[Q18] 模糊匹配
来源：http://blog.vehdjk.com/Article/details/gketadjfn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gsfnirwkr.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gktaghgec.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gyzomgujq.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/ggoervxcy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gfelggoyx.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gtvxkecew.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gffecdcdg.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gaqyxaldt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gkirvyaef.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gqhdhdsos.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gjfpwesty.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/gqnowhgeo.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/gabackbku.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/gxgurrkbg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gcgfvrequ.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gzaxgixdx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/guexmhsub.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gbttoanlt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gdwdiffiu.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gkjaipjng.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gtmemnhcu.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gdxqcvjyh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/giuwvobus.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gzoyfwdfr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gxzltjppg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gwsixegop.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/ghwpherwc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gkusogtwz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gskryqjmh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gobnnxmoq.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gvqhwxfge.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gdcplfoza.sHtML

[Q34] 每组取第一条
来源：http://m.share.epnwcf.com/Article/details/gtjhdbpse.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gqoatefvr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gnqggvnlh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gfliqwhqc.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/guhsnntih.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gxusvknss.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/guymzfdbz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gfyypiwva.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/ghpuarnlu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/gvsnvfdwv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/gsktrmjfb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gidmfvbjb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/glyeuknvf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gzqwfwsdh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.vehdjk.com/Article/details/gqxswhkss.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gneexxdmq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gsploljng.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gfqieulzg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gzejwlftg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gzlqqfzfe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/ghiazdrns.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gmngvesqp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.bbcook.cn/Article/details/gvnevizwf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/guphszfqg.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gjxknhjgo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gbxtjrirn.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/ghuiiwvaw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/gzgbododx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/guekmupdq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gexpwbbwj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/gikszjxkb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/galalfger.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gawofzfpt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/glikyxwrt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gzqpqxrqs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzrzhwmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/giphjeusy.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/givfnukme.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gghizwdex.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/ginjibtol.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gywkicxks.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gldulmdel.sHtML


<!-- 参考信息 -->