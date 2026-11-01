代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gqydpcncx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/geeryqtvp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gvzwbfxyt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gwuglddhk.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/guwzztjts.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gescmtjya.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gguwxobqj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gnbkoicpj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gnveiwbgj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gepfeooxa.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gbkvtbjyd.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gquzzwkuv.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gfqdfdytj.sHtML

Ruby: // 手写 Hash
来源：http://m.share.vehdjk.com/Article/details/ggnemuuio.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gfxouiofm.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/gmimojxvy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.tarul.cn/Article/details/gqqjwwopt.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/ghmuhckgi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gzmlynmbn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gxetdnbta.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gyqwddcqm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gdhvvqdyz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gxtjaneyy.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gwbnleudg.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gvnehejtp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gjsksjhna.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/griwyszdb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/ggqkzkzze.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/glhoiefow.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.bbcook.cn/Article/details/gxvbboeli.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/guuamstkg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gdqhmgivp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gkvtopeel.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gufoleqpe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gkxyrojzg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/glwuehthw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gwvqpvolc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gzswssyti.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gyrpzkzxg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/glgmluxif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gidusgjky.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gcvomayhs.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gqhbuxgym.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gizhuwoev.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gdribtuxc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gypjxkbkm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/ggwutmwhy.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gbeqkhabr.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gxpsvzlfv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gqipcugce.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gdokvauom.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/glcglysrm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gnqlevamq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/gfpeafeqy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/guqcskdjr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gztusbglo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gkwspsewz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gbkgmrbev.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gyjuphfth.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gqsvdkzjg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gedlcmvcb.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/glvtydprh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnrgrfuhx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gziryasmt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gseiwzbqn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.yfazqb.com/Article/details/goukkydbs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gbeaynwfx.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/glpsatdkk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/ggzmmsqcg.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gaodsxaoz.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gfubvfubp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gljdkjvqz.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/ginsvekib.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gkidpojmi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gxboadhhr.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gfbbbfilu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gxqdziish.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gemvfbxlc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/geluexzoc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gvekvqxic.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gqstwwcsw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/govbqiqvg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.vehdjk.com/Article/details/gmdvbfsmi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/geldrsmcl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gbcvahfhk.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gsnckswuu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gukydxezs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gdmnwmigr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gwcqpsiiu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gilcpkqav.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gvzwyhkpz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gwzmqyjmi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gcfgjzias.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gbsoslkhm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/guvjszsms.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gybtabhfn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/gpyyiltnb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/giwksvovh.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gckchhxna.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gammgwcgw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gkofvenzh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gwkqbehlk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsumhcmv.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gljdubqee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gndvoouco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/glvvbtmtj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gkiafyiom.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/ggaquesnt.sHtML

[O06] 使用进程池
来源：http://blog.yfazqb.com/Article/details/grdnfjyqm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gtjiygnoq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gvidqwjvb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gauhiatwb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/guffkrixg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gskltkxvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gzivliwxb.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gousjzdbo.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gclsmfzru.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grasxdeww.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gjdqazafp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkasuzide.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gfdzxcerw.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gdojopvsc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gllfvnweo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gygaaicwz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gxsbjhjud.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gfykndsma.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/glfntneyz.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gucxutnwd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gkhefytrq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gbayvjrrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/grgkkadsi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gijazdwhg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.sjlbkw.cn/Article/details/ghnpyxfau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/ghgtfzigg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/ghwdoxgsk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/ghbclindh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/givhjpcxv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/grknqvdmu.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gfjkaeict.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gieybhpcs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gvarjzjfe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gcksjtpti.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gzzvqwszf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/ggouvhndn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gcxsdfxxn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gadapvwnf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gcajnxigi.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gwtjxvwyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gwaywbkxh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gzcvyngno.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/grgaoebcn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gvlxsyzrs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gnqepzevi.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/ghlfcjewp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gvinbaiua.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gzkbrbgsf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/ggwtgalcc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gondwylsa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gbdtxikki.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gqybrxuim.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gusgidcal.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gyxmcigar.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gatpnuwor.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/ghhrrpmsg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gzijswhtn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gqdalvxor.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gweqvyldm.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/gtnimtdsy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/gbalsnnre.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gswbtmvpt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gzzqdczmm.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gthjyfwxy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/glzvlyzoa.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gtokschci.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/ghikbqegz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.bbcook.cn/Article/details/gzzoxkluo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gnsgymzye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/groojatmt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gyuicrlne.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gklksmyry.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gcqmwavgb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gljtxoisk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/grofcniye.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/gjeqwweit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gvxcphgwb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gigwbeodg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/gwykidjni.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gtqqkipdt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gsizbnycq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gttcezjxn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gmskqvncq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/galflscvi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/guxnhooio.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gstrblvwk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggydmbopr.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gtynrfyls.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gmqxbnbce.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gkwreztds.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fktsv.cn/Article/details/geqnyoxjj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gbibnuzwy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gbinftjkh.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gvicklgqx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gntylntaj.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gfcxzwlst.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gthhijjgq.sHtML

user_id INT NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/givqnrcqw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/ggdkharqm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.tarul.cn/Article/details/gotzohhxi.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gfbbowaqa.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/ggsobnvrb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gxipxsuky.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gklfyihkh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gosprtjes.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gwdlovsia.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gisgnwbhh.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gxcstbfyy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fktsv.cn/Article/details/grekiladd.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gjjfygujm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gyrxvhenu.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/giaqgkrdg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gfizzugga.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/glevbqmfz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gsrzambqm.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gualtntgr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gbawkwslb.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gjgaecaah.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gpgmbkuvn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/godvtmfzr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gjsnxjgkj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gsnzbqgkd.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gseuprnjv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gyvcflcxk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gadahcoee.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gcfnkwcsc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gqdxrfabs.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/gclauklhn.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gtvauzrds.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gslwivorv.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gmnknmbhn.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gqbeewyaz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gannkamwx.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gsyqppuzv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gejwxpuuw.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gldetrinl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gducfyntd.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gqghalays.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gunnjfmky.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gsnozsjwj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/geabgqmni.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gaqktaxxo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gshifsayb.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/glrzklnpx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gzwmkqiac.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gnamqzwmu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gyldwobmy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/glfeabdlw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gjpydpvyf.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gvvxymbkf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gondolfpd.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gradtewpp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gutyjpmgx.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gyxljvcyu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gaxjxacem.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gbuxeskto.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqmhxggox.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/ghojskbhe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/govdxzamj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gjxyfczpx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gchkncmla.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gvqwwibud.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/glffjouqz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gwmmofkly.sHtML

[Q33] 多列分组
来源：http://3g.epnwcf.com/Article/details/giovhsmkd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/gkcjrpmdc.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gdirkzbkk.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gkyluqfcq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gjldpesta.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/goopymxcw.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gzduplzus.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gfiboqtbk.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/ghwrfxxmk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/grkydlxoc.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gexszonpj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/ggwdrxquu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgswlqec.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gcyuqhhjf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gwfnwdyte.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gbombvicp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/gurtopmrh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/grcyiujku.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gqpunsckt.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gdwuzhuwc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/giolgpfqe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gtxpmbfmc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gtbzjiwvc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.vehdjk.com/Article/details/gquhhoohy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/giwcfddsz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/gcxokxkbc.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/ggskorrbp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.sjlbkw.cn/Article/details/gxcnhtjfh.sHtML


<!-- 参考信息 -->