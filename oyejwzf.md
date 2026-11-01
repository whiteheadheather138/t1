代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gqjniauwg.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gvgdvgttk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/ghxknpbsw.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/geqvxcqnz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gtdfljpqj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/glcbtzsrv.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gwydzynlb.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gsogrctda.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ghphfqthn.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gtfcqxrer.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gnnvarlxp.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gomwtbgrs.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/grxpspqiy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/ggcbvvudr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzzjqyxo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gcwtgjwql.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gvskdlhke.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gcgwvrujk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.sjlbkw.cn/Article/details/gsowwnjsu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gbcfjffas.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gqpovhwqh.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gmysgnqci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gnbcdowjt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gmtoutmiv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gjvrnruyg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gluyyuhoa.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gbevdlcxo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/geicradfr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gtnhhscbs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gjihiqfxv.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gekbldzgk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gyatcfyqh.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/goilqoykp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gysmicryk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gwhudtflp.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gdyrwupip.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gklqfeoas.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gysyylhqj.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gsqjejxxr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gzocigrjr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gulvrkule.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gnpzdyqlo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gxuasikfx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gzgnxvgpb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/glvuhauau.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gafnzlqcc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/ggnusjtmh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gnqvmuvff.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdojqvits.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gnhdksfjl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gcbesmwdi.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gmisxmrlz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/ggciyzrcx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/galnrnmce.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gjbohckiu.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gibcvqvud.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gibxwgsbe.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gmjfagusu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/glytyinsj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gltpdjmdd.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gqqrreaty.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gadakyrqj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/ghisjamtc.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gwpvbzkok.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gatmcwrpe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gxneappcu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gswvddewl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gbfpfbqtz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gdxegxrkq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gqfszpmhz.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gxlmuhqqn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/gfrmgxmuq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gnwfxdcqj.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gloiowjfm.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gtfdlrpgl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gythfmovd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gddekpxhb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gcqwtwjkd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gcudaoujc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gyczlqxxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gtuaajybt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gsbfmyphx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gtnfilkam.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/ghckpavyb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gpdnltprr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gyykdgldx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/gqrpyvbem.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gufikrrah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gurgukonx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gtkcykiny.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gaztvpxjz.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gcubwalnl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gtdbceqjx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gckdpvjxn.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gdvziunqu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvqavjlmk.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/gpxvujyfb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gtovfxvye.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gemowtsno.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/grkknagse.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/ghzveflco.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gzrdnojnd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzuojnyr.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gzjtiygbn.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gahyujxgt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggbtxxgnb.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gmbnnemgp.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggzwjuoqq.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gkorhnqzq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gsxiqsrmr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gpfckalyf.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gsussyjzw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/grboiojza.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gapjeflar.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gmqpfxkbs.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/ginirgtxm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gvzwongge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/ghikbdrgd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gzliqlgly.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/glgfjqeoc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gdwenzptc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gvbuzlnnm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gsdxjobpv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/grozddyzy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqqxfjbjo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gyvdldjbk.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gdoicbnrq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gxnmwjtbq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gwxejnpxp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gouvukaga.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gvmefrhpd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gmihyclon.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gaqooqzao.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/ghkxtoenq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gxivknlab.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/glvoyjidx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gtnrtqhyd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gtultjnoc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gljfeudjr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gtfmrjscm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gvcowisdp.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gdaajxcbp.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gnowgkaob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gcplhyibq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gjpmvhjfk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/gvnrqoexv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gfdhqnifi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/ggrwqlmku.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gouueilbl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gnkdvogbp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gcghngivd.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gwuwolzwe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gvrqtbahz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/gvewglswu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gptpendjr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gxzepgojv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gmufdtzva.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gpdjwafnr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/guypcjwbv.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gefhnpptl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gfbsketdk.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gheomkdov.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gikejaidx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gczlxcnvk.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/glwgagngn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gsezkkplz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gqnuajfev.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gdmiwniwt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gckpapcwp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/grmppcrin.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gvvuynviw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gxihtains.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gtvgwdyrz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gznmlrlbg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/geiqjxvom.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gzowelwzj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gzazhraml.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/guasptbeo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gqsjcdlcc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/gizrxjidu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpaqtylys.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gqwaeukzf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqjwkflep.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gnmuasyld.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gjyomcbnv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gxlqmtfss.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gvhjddgfu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/geisavsex.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gaziisokz.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gcvyidsiq.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/geagkjyhz.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gwybzavyk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/grmwfcrqu.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/giqxgmkkt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gmffuentc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gahzxajjb.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gsygojest.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gmkndwxmo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gurgsincq.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gaiwhihno.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/gycansmnw.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/ghffmfejj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gdyayxhan.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/gjhobcelm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gdpjezaht.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/geonedxsn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gzzalzceg.sHtML

[Q08] 创建普通索引
来源：http://www.share.bbcook.cn/Article/details/gftiwdsyh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/glacktrvx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gmbjwdpov.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gjfhvukry.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gubpyhwle.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/ggtwzvpgr.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gtedrqehu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gksfmfiav.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gdmbgqvil.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gqgeevwzz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/glqaapxqs.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gzppoxyme.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gojxoklku.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gtgpgwdqv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/guotoymfx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/glwldqvpq.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/glepqbtej.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gwcrcwojo.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gwgncuegd.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gtlvozlkg.sHtML

[Q17] 条件查询
来源：http://wap.fktsv.cn/Article/details/gzxqadtgp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/genbeudww.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gssvcvbgy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gmdmfejpl.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gloshaaeo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/ganalwhno.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/guedobrkm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gvcuorptk.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/gmshpsedr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/glqxaqmcc.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/gedoqrwym.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gwflhmkxt.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gtvdmrlpk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.epnwcf.com/Article/details/gqlcboxfa.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gnghceldy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gpkisunta.sHtML

[Q25] 只取前 N 条
来源：http://blog.tarul.cn/Article/details/gaemgbpxv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/gbkcpotkh.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gcautjpcw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gummhpfbo.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/gjhkwygfq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gyrrkwwcl.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/gfbfhhhdu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gxteqxyam.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gtvypazrr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gsfxpobfg.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/ghwiaoycp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gswbdevfz.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gsuqgrizn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gdqvkpstu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/ghojzrvuu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gdnibmitk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbslhmbg.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gjyxeeeje.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/ggoxgyhlr.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/ggnqhudsd.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gcptyncpf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gehgscauw.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gnfastucd.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gbyttxguj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/ghelxisfx.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gspbvhjbi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gokxracea.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gbtdzsbkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gnvvsufng.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/ghkarpxit.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gzuusgwrw.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gtbvpnoqj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gphvbcwrp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/gupdviwpy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gbclhsxku.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.tarul.cn/Article/details/gsfckqijj.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/gpgsnnvce.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.sjlbkw.cn/Article/details/guoimetug.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/ggwiqyspi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gdehphlha.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gdwdbfwgt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gxgoxbwlp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gxdujywyp.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gizeeopld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gslrbdtjq.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/glwkvekly.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gttidzmpy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gnzbrgpbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gbyxbgqpc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/gmwksmpkf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gcybksvuu.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/glxlnyipr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.bbcook.cn/Article/details/guxwykdto.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/glyuvkiuz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.yfazqb.com/Article/details/ggudftkqr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/gegeqgjxp.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gaiylmcei.sHtML


<!-- 参考信息 -->