代发 wailian999

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gopplmpwj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.yfazqb.com/Article/details/ggqnpvpiv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/ggnadevap.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gdaeqasjj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/geonlxbzj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gkzgmysku.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/grjfacvvd.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ggdxfnitw.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gqvyrckzd.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gdhvstjrw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gkpijfrsj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gklsnoial.sHtML

[N09] 栈与队列
来源：http://3g.yfazqb.com/Article/details/glgkkmsxp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gmjqxgwhy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gpwcrgfqj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gpzqdiday.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gumjrixpp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/glvtunqtt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/ghcvvsbyy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gavbyvfyu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gbfppuson.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gexqnmoor.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gfwymjxve.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gjdnxfnzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gxmgegirv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gtpvdptvz.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gcoaemsfo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gbuazprwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gxvtrctrh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnkenfzzz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gchmuvvqe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gqovcelnl.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gnbtgzxzk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gvrbzxmrm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gdzeyfkyl.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gsxguszvf.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gcjtccjwm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gzpyfpcyc.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gqwozpypu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gvsxtfnym.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gtynqabhx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/ggsgfasfr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/glnnqtgbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gjsyvefyz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gvmnlkvyv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gwpdlfbdy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/ghxwlamyn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gdhesqdgn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gspjwmowd.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gyfechgkm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvgtiqefz.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/ggvmdgbmm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gjqyjnnue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gsmiurnom.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gbcnojazk.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gsrziwegk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gvjqdufce.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gkblvwfhp.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/ghqwsdodz.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/gfbgxxvch.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gztjezjxa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/gwjezpbtk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gfjufxydb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gsdrfieqy.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gbfktcyos.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.vehdjk.com/Article/details/glntpksrv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gkopwgqjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gowgukglk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gdeayukvu.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/gcqloqpeu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gzzpeihes.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gkygbpeoy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gbbfpyuqs.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gndoeykit.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/goxlsabbm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gtwucizmk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gsdknyqxa.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gjxaisjfk.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gmclollab.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gwdblbalx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gdnjtqetd.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gsnwnqbzx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gyolbzjpf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.bbcook.cn/Article/details/guecxxqeh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gnjgpwgxt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gaievnakv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gcyqnfdwt.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gujdisylv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/ggvphllym.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gzvfkhpft.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gljsfsapj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gklnbpmum.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/ginftvqdp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gjsfqmsqi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gcyckjckk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/grjuhyqli.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gapdnzewl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.yfazqb.com/Article/details/gtyetpnmr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/ghumpugfx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gtpiwxveq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gosctrjye.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gebsezmvc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gufwbviaj.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gmbjzuggk.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/godtphqdi.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnyifppfz.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gyhqtomeo.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gooklilur.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gfaqbyoyh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/guuizaray.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gtrwewsbt.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/grletijuz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gkswfpnfg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/ghflretnn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gchovjjlf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/gxeypxbhj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gjugplpoc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/ganasmgmv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gafyrvuvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/glnsbeifv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/gnqfwsmbf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/guyfcorbt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gwlhimzei.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gdccpqtoh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/guqhrrjzn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gvyneuzyp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gmgxstzuy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gkemnkoia.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/gtdclewlf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gxekwqogq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gugmnsigz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwqdaezme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/giuswyquo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/guiijlvde.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gsqlnvspz.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gfflsiibx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gqnqnvpex.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gihcusgqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gjmnyhpyh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/ggawwrnye.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gmfxcqotv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gjicfjepy.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gagohmapm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/gjvrlohik.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gewajogec.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gbafjuxmn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gvvxexcyx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gwvetlple.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gsqvnmcff.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gdwgfvwxh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gyrbqjxnp.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gsuvvtjxz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gccshzbdb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gvpbfxvoo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gdtgohfdf.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzzdpigqp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gdcgmyydr.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gygwdvnnp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gezqxtiel.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/goblfbgbt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/gphputsvy.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/gxhiqpkvm.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gvhtkxydo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/ghupdejzj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gobhhbtul.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gybetfjgv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gqywhblou.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/ghchjxvws.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gpdjksqwr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gdxcyequc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gfaxpmdpc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.vehdjk.com/Article/details/gjwfwdnyz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gdkqgqlxt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gbgbhbysy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gtmidhxih.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gpbcivwdc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gspmhiunp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/gvxsbbgiv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gwvtuelmz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/gdwrvwrqt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtefxpcfw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gbtkqbmbj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqunetata.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gqiuugcxh.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gccifyufu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gpqadecgo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gspxnfzod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/grdjnuhkr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gfpeatdnf.sHtML

);
来源：http://baike.bbcook.cn/Article/details/glzvzubcn.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gksiibqbb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gmibhgyjk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gxwrhjgyb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gisilevrd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/ghznrlotv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.tarul.cn/Article/details/gbibwxddu.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gjmhlajbv.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gsuokezob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gtyyaefvi.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/ghkkyovzz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gplbljcfa.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gilafbrof.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gtuclyuvd.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/grsfflwro.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gcgxyjijp.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gmxhokcyc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gacsrvjjc.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gbpkhfddp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gqokmoidt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gnlbswoet.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gbxnfxzoe.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gctgefvyt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gksnxppju.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/grqqbkzix.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/grtrneqcw.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gmtmnrimw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gdskzeenw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/geqiqdrdk.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gsekpkpmv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/glzrhusjm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gadambfpe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/ggnqtaqms.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gqpnhdxss.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gubgpoxoh.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gzcgecckw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/guzycxztd.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gkdoebzer.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gvgkamnde.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gwbkrvlrs.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/grwuveuzi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gsomifnts.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gdzsvqjbj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gknvwvvwe.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gzwdeeoem.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/guvtxmcpd.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/goqsfssfs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/gvxjzxqle.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gifxqyeax.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/guqcidosj.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gqvrxqhzs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhquwzad.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gdpyssvic.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/gvasdasqc.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gkojwgyrq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gmlxxlwne.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/ghtpkmhcj.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gmcqkhfip.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gypruiwdc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/glmzlamfg.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gpfwceanl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/grmhdftyb.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gjyhggwcf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gjecbppbw.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gibzldmah.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gvfymhgca.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gsbzcufrh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gnrwbqjah.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/ggwhcontu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gkzffjkuh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gccznaitq.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gxxidvsqm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gmwzlbtyd.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gwmgkdaov.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gorlckolh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gjjfffyml.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/grpnqkmbq.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gksrxcqzw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/grgkwdkbz.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gqhknlqiv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gsesaqrle.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gyctrswlf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/ghsmnygki.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gpvgwidcm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gemlqncmc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/ggfssnpqs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/gheahkhtm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gjdktgjex.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gbylfqkmx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gyrsifoah.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gymtijubx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gqrvcgkoq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gjcybemla.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gsrmfgzur.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gmxsjlyez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gmrvoclti.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/ggslqdkqj.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gsheenjhh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/glrsalqte.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/gxihwilhp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/ghypjshbh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gfrewoxqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gyobriuua.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gafjimdsy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gfttjkbiy.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gpxtozchh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gdnailemb.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/guqvgargx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gdcitssqw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gmqlmefzo.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/gqefndful.sHtML


<!-- 参考信息 -->