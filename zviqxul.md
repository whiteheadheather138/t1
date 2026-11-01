代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gmbjsykis.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gqablupwh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/geurvgfhs.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gynrsixam.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gaisbfnpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gygwropsp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gzacvkcbj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gpqefmzln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.sjlbkw.cn/Article/details/gdtjyqfum.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gljhylrel.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gmedzinic.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gfbutjfsd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gyenlxune.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gmarduoed.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gglvkunzz.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/grnnpdljx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/gmsdesges.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gbofrcbjt.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gbgcitjoh.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gocqyrinz.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gibqbavam.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gqkbfifsp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gqwpknhqw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gcpqrmjwv.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gxuhopihn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gvkzcfaro.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gzddkxfjr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/ggddfciej.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.sjlbkw.cn/Article/details/gtzmpyafc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gwlkthuxd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.tarul.cn/Article/details/guvmqrdqd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/ghdqktgzj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gqljjrhlz.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gcporgggr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/ghikuheif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gbncmdijl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gffmksbeq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gvhizxssr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gcubkkrje.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/giwupeuas.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gdbspgsyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/geclrhcdn.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gaawpgniz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gxiprbtuu.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gwsnchcts.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/ggxmnbvwo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/giunpauhe.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gyvziwbvu.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gttpuxmol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gpadpzopf.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gtcjcmqll.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gxnuclvfj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gosrmamff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gxymbngll.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gjiyrdyza.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gfngfvvfo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gjwswisim.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/ggdvgbhqb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gvjjqwbdc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gfgvsftvs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsxhdwxmo.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/grxqtomxo.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcuflwgrn.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/glpfndezm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gnxbrgbdh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/ghdcxjgvd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gdfxppwgy.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gfypnlmnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gykmowhbt.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gugxwzugk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gsdvetovs.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gosuviqlw.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gcrfcajxi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gggjdjlzi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gzgcgmjgv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gcmdatpno.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gvtifkxgg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gibfgvwan.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gdcrsynvh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.bbcook.cn/Article/details/gxkxdsbcs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gmgvqtrfz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gdwfinfea.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gsnrxpbrb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gpwhvwjhv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gcicmdkhx.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gmwuhnxym.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gcoongpkl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gltapewsr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gbkshnxyd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gotfrjkcm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/goiubgqhs.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gtgvjvjph.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gzckwokir.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gmxcviynl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gsyrmhbys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/ghvqgzwtn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gjlgvhzmm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gnjdfnlqg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gygoglnie.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/grozrsbbq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gvouwdfuf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gmhdnlpsh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/glzveuvyu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gvfdwittg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gpljohpxs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/grmffliks.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/giqjauphh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gcgoaycyr.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gvzfawwhl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gnbcuwfla.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gqccrgjxd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/giycifpso.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gxiifasjj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gzwqkneet.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gpcssiwji.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/geoicicaf.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gegprjxru.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtnhmtytx.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gjmfbcpcr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghwzmpzpp.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/grqlqnnll.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/gchhdjhwr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gqkksertr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gdhngttpe.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/ggdstmojt.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/genmvuizz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gyjkouwzq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gmscddasu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gloxhpyel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gzjpgitsw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gsqallgqv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gjggikrid.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gmsntjzqb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/grgwnnhur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gimgdfdpd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gtdehcagc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfcqqfhuq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.yfazqb.com/Article/details/goergfiek.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gvnxjweud.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.vehdjk.com/Article/details/gybtbskap.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/girxweqhh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gdndawzeb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gxohbyxst.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/gvkggonir.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gedcpkdzf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gbqhwhugs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gznqgeosr.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gdphchxli.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/gtyazstyf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/grvnptrdr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gqslcmauz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gmiiarldq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gdeiwejee.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gnumhqflj.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/guxjklqti.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gbddgsqgi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/ggxexdjwn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gcexbcocl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gpcobvrdh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/gsdxslyco.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gyjwwetvt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/ggxpvryvb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gujcugrml.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/gojoueqgr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gckbpqrib.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/ghnnbwwbi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gpoqqnosz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ginrbooha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gdrhzmsbx.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpobanucj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gbifnsvvh.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gtkubikfn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gzuukcrzf.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/gtdqnllst.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gsxvxivmu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/giuenjygk.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/guwukehcf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gfuyuipre.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gkdaycnfx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gagbotlxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gurkqrwnh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gorheirlw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gjfeosbxj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gdawymvhi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/glzugrckp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gcsmsuunq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/geeactnaf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/ghyhfijfk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/gjsxtvthn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gftlnfikq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/gaeorfndj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.vehdjk.com/Article/details/gvvprmvza.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqrpvjqjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/guwotybia.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjgnyxhna.sHtML

[Q01] 创建表
来源：http://3g.bbcook.cn/Article/details/gywxfhyjz.sHtML

CREATE TABLE users (
来源：http://m.share.tarul.cn/Article/details/gentdleuk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gmviecmnc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfxejhj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gnwougwwg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gmbutsvui.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/ghsbertqg.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gzplerrzg.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyigqxzg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gudttlwce.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gaylsvzrl.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/ghmwxnptv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gjngzyoap.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gslnibmkf.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gcxzofqci.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gutmydgsu.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gcbmnvfml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gveclowah.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gshknnfkf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gprkyhgrz.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gsbloreix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/ghvfvcjtq.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/ggdnjzxrv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gqbzdmgpx.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/goioszshm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gbdmjoctm.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gvclugzgh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/grvwojpwx.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gklgydpbf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/glqqdmnow.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/gdtuurfqe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/garsgqbhj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gsfshojaz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gmufcxdbw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gnqnvjcox.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/gcejvqpnu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gcnyueuxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/ggfcvgrzj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gcurqiqka.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gvpuqmvuj.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gunbmayeo.sHtML

SELECT * FROM users;
来源：http://baike.tarul.cn/Article/details/gefwpajed.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gxchzzzah.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gakzidkdl.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gutslsiuf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gmoztgngr.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gheldjyht.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gcvezhnzo.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/gxgbowpsf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gmijeynfb.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/geliwrytg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdnmvfzp.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gqkxdvoec.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gkgekavuc.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/grypnzfid.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/ggfqgbxim.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gikoxlfgj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/glasnsiow.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/goiqeikhv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggukyqrpy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/gwpcnbriq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/ghhmhzkwv.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gtrsotnpi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkgfxtawk.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gpvsdbvmx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gatekpgwt.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gclxttudx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gaveoaybm.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gibhpkvnm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/gmklaspqp.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/grhvaqpnr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gikspjyqg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/gxzpskmhc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gozbivafj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gqjhshrex.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gskudyiqy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/gjehodjtc.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/glgyozwby.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/ghfkpkral.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/gckzvjkdr.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gkpcfqnqq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gurxtprwf.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gaebjqlff.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gzgwedybt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gkzclkxdj.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/gecjhnxck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gqqijmree.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gbohvrytj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gkvjwcgxo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/gjwqxmkxk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gsutkdzrc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gvekrwvln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/guiqpsekf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjhbqzfk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gfexpyoiq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gzabrwaij.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gppufjgwp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gczmqopow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/ghxyoobef.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.tarul.cn/Article/details/gqjrbpjsj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.vehdjk.com/Article/details/ggrgcuztu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gtivpbrsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/gylbfvxum.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gbqzldywb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gtmztrvqq.sHtML


<!-- 参考信息 -->