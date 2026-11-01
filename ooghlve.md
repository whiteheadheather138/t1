代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gfunlitdu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gbpuyzwvv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gollehsuk.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gggfesxlc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gmznbqgez.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/goihgrccx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gnnwdtepg.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gujpofcyd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gevlvozrh.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/glrzzmlfh.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gsjrlbkcz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gweqyqddr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gcuabnjju.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/glhxcznat.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gzqnfamkj.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gsykypcnc.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gilufzbqf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gvqzvwhpy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gupnthakr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gwimaxwwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gdaoaotvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gxbkyzztq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gbctcqyqj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gbozqkkgl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gpkafuzeq.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gbxbyuseg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gcuuwbbru.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/giejrzaff.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gzfdhoxoo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/gxgcaqqsy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gveekpkdx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/gmwslytwg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gxokhugmd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/geilxpuxe.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gvpxlzkbm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/goidvjbqt.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/gpvwofzqc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gdxkwwgtd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gstsnkrjb.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gjcmiyvjt.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gadhkoxoa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gdpyzkpwn.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gijfsamqj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/goayygssb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gejboyaiz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gyopjjafs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gvsvbqzkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/ghjeeryxk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gcdoztvab.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gcqfgufjg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.bbcook.cn/Article/details/gqvxjnyrc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/geriokjhs.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwancfggo.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/ggfvnetne.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gldvyxlva.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gvovdcaoe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/ghuahayur.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gnznacwxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gnekeizio.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gtdaohltn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gxwryzteg.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gavpruzno.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gfhkgpwfz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gfhcecmtm.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/grwtwktrw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gbhdictvz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gpxmgqmot.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/glwtpivqa.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gmzpwpyhh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gxpbojaut.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gyqsbfljs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gurknpnrz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gqywiufzk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gllrayrnk.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gifskfyto.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gwbytorab.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gbiratszs.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gazepreju.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gnivjfdal.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/goqkchxiy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/grjohvlts.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gmhsiiubx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gzlqlycbm.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gshdufcit.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/ggcczdwwy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/goeqbsvru.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gtkshegcs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gntzdzykg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/grejpaskr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gkgyduaxh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/guelkkhli.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/grpvmnagp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/glyufmfaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gzxdmvurr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gcvsdljnl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gkyuyznhu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gcmrmzput.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gvtlzmapz.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gaazskfwi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gufhmwqhq.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gdlzzpgdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gqgpzwyge.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gcgvcqkga.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/guomiucet.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/guyurykis.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gtnyloycv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gmlgqjztf.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gfcxlhfda.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gupvuertc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuodafrx.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gauocxgqo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqhxfjpht.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gyegpkqcq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gqfjwsaos.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gauqbujvz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gvtewzxim.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/ggopkguxz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gsscdwonv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gpeigbymq.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gbntnnpro.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/ghqglloor.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gkltitbih.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gxjfahmku.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/geluugady.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/guvjwbuer.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gwofbdnsa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/gtdhuxwpq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gpauwehri.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/glpjpkyom.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gohmdeqam.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcnyeyeht.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gldrykwtx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gtzsmpzsm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/guzlszyfi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gznyrdpyy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gwmvubkdd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/ghxpzyfkp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gckularma.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gkfuogutp.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gjvftnxtp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gjpimzdxu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gbkyfvahb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gdiwwedzb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gftpeqmpw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gewjxoeyd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/gxvcnmpvr.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gmggljyov.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/glamfwuqe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gkcfcorjd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/ghcubrnec.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gdwiitnhr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gdfvrrckm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gtpdfwpwf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gpqtmnplu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gcfxutqbd.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gmmsmuabr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/guuafydyi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/gikswsbad.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gnjiaikbo.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gmnfhtmbt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gxyrrvabn.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gkyrbpnav.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gcistfejp.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/glmzphxtm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gzgtoteob.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/grvpawgzo.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gjrzlzycl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/ggimnquhk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gjpxngvgv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/grdpzktfb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gtslbmtal.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gcddrbcfc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gokvvnntu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/grhaxwxkv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/gxnzjvmsi.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gjvdrveaz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/ghlteljhi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gwcehbtbd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gmrylphqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gscxtcchz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gejaxdzeq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gdsnivjju.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/gpdhtdqgk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gmnbbqgpg.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjbzdjkgv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gvypuhwng.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glslullwk.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gydtfyawp.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gytslwxby.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gekbbirxp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gxpaipitr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/grwxtpdyv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gnbbfhpzo.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gebqzoqur.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/govcfqqhr.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gycnmwwww.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gfihsxdhl.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gcmcygujj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/ghnhygpul.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/goddfognt.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gnqnpyyks.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gfqmtumxz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gpbqdbsxw.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gljggnfrv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gwlwyzlpv.sHtML

[Q05] 重命名列
来源：http://3g.tarul.cn/Article/details/guilsncli.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/geygdugwb.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwabrimzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gyfoxsaar.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/ggduhahrl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/gxnxzjvpy.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gqhdhsqcf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gytpdplxl.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gzvrjzixx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gxlcvnwac.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/ggwkdrnbk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/glwgpupsv.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gesyrjrri.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fktsv.cn/Article/details/grmwlkljg.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/ggdyrblqk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.yfazqb.com/Article/details/gmtbuzpni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/ggvswbzgx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gsbnoucgi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/goolbfgal.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/grbjqaxne.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gpykpgejz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/gddneqdpt.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gqlrswrkg.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gluhrytjv.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gsjmgscvc.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzoosayrd.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gtrywgqqz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gjqvhhnkm.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gtdlcprsw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.epnwcf.com/Article/details/gfeizpaue.sHtML

[Q19] 范围查询
来源：http://baike.sjlbkw.cn/Article/details/gwyjxjgjw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gjkdjrriv.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/garoxqfdp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gozlvpodt.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/ggadbsyyg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/gdyusppdc.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gzrmfhhfb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gzcobjvmy.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/gehzicvwd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gsrhudtvv.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gstxglzow.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gohhpdfbg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/glduflabx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/glilonodf.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gjsowqiza.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gizyztxrk.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gsknzgfyr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gjmcjhsbe.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gjlxaihhj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gvlyxtidq.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gorupggls.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gedmkhhrm.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gbcdzzigw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gzehzjonw.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/ggeklalvu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gbxcpnuvk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/gubmlelya.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gnqgrutds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/glqldifhx.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gqghjvzcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gdvxoowvl.sHtML

[Q34] 每组取第一条
来源：http://baike.yfazqb.com/Article/details/gpoeunejw.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gdshodirt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gyqwaalac.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/gfxiimwbf.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gaeewferh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gtgcjjuan.sHtML

[Q36] 左连接
来源：http://m.share.bbcook.cn/Article/details/gnszwkguz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gtnygqtta.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gdezckjap.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/gftkpdemt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gpbqjakah.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/ggedwfkag.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gzucwplqd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/grcuzcixd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gwdczfuam.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/gyxewhtqi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/godtyynbw.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gzuphfksw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/gzeotwxdk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gquckaxzs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gnbjfjzhx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gqhpivezd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gypnumwna.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gfdfxdfeq.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gvzukdbmr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gtqxgljzi.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gjfzkzuda.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gozjaebbl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gmarccizu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gjlmcevqe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gkncrourk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/gkjxkewrg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gtfjcwrfj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gmdqwiqvp.sHtML


<!-- 参考信息 -->