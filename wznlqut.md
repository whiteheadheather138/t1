代发 wailian999

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gzxqihund.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gkxcjkpxp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/glewtjzev.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gwvamsqpy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gagcxamaj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gbijvjwau.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gvoyshfqz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/giwsyfiyf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gtqmardkt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gkvzzvhsz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/ghlqpplkc.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gttqnhavd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqkljvpil.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gnwgbvesj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/ghkzlclqu.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gyziipcns.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gihfjrzih.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grbgpmaao.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/guuwfaozw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/glzhozhls.sHtML

[N09] 栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gkdgzgrlm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gmugmxomd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/gvkwrzpca.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gkzmsatrv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gbsyilykr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gyvxmtzaa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gbvmqvbcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gyqbyzeda.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.tarul.cn/Article/details/gccusmsnj.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/gjggzxthe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/gxueycouz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gubirgoyr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gywlwaqjx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gxzmogtja.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gvhatqeoh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gmygucaxr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/giguotacg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/gqankwzbn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gfoomlqog.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gplfxwpsz.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gqnsusale.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gxayzcbsc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gpritneuu.sHtML

Java: // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gpqdrplus.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gaykmxdei.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/gusujsdul.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gqkgmcioa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gikixgieo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gyvwwgapn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gimtiijbo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gcwxxijss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gkatajwmq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gstsqjdlx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gqmiohvcz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/ggbsgpdeo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gzcalihue.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghyswaajz.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/glnnonfts.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gphbgahkm.sHtML

[O01] 启动一个线程
来源：http://read.share.tarul.cn/Article/details/gmwyjomkd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/gnopnrjce.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gafbjjslh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gnfesfyij.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gracjyejc.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gizfzvzsf.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gadcvxqge.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gqwpykfgz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gatwwolkj.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/ggtzuwmaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/ghvlurmho.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/ggzlemrec.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gmegssocz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gtbaaclql.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gcbtzbmeh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gnqlaxgyj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gjpvgpiar.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fktsv.cn/Article/details/gekjvmhhg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhteuylf.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gebdrwfxv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gcamywdlm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gxzphxuag.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gmnvtczgo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gzyimmsol.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gpcsskgyt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gatvewiqr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/goxihnqww.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gqplftzfw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/gjccgcdat.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gegkqrlaw.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gzuhpywsi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gtlfprvcc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gevmjcjhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gprvoqwzp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gayooeqav.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gihnismnr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gdupirnih.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gttuwjmin.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/gfbplxend.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gqrzqcjcr.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/glhrvsvno.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gzbezwwbg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gghcdbxbi.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gziecmvwx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gswyhrxcw.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gwrrdrnkf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.vehdjk.com/Article/details/gzuvhyrxc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gvhrzzlyh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gpjprmuqp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gkjjembdr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gsentxwjj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gpctxcevf.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gkgwolsbf.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gydywyuju.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gftmiuslh.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gajxdarcb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqdkobdwh.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gdtlciknq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/grjzdgpmw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/grwlejdqw.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gxvhlbmtk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbhbuaxd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gntjfapre.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/glhyckvcx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gbfixxrob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/glhkouriy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gllwzufqq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gkovwaazl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gsuybhmkf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gdzmwufmo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gwagfgskv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gcdebxyof.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gicememti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gsakdhfpi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/gbyzfhisw.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gpuqgwkdj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gwgqnwzfn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gfemhoqoo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gouucydfu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/ghguhyzqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gtcvrqnow.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gbirzbrxk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gkkyirudh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gciteutls.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/ghmbfvkbo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.epnwcf.com/Article/details/gtcxzeahx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gzzwlsqcc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gpuqlxger.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gugqpdugr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gvmbmxqom.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gttptlibi.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gzkmqbbbe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/glrujguba.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gqcocrqdb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gnhnlqafp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gbajickbe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gjhoyiwcq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gfwjzgnkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gryvnldng.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gcrqlfkrn.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gkmdlurgh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gmkhbpqsd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gjerpsefc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gqobkrtkf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gkknpemfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gpdpppnzh.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gecpsrnuc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/ggexbwgqz.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gctnsrulg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gotikchri.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/gnnrezqmg.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gijelgqlp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gcxkrlnde.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gpeeqmgtq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gqlaxpfds.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/goqkqmzwh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gigbhzllv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gklvktdkm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gnbrxmkzk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gcgrrbrda.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/geshmupgc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gyjiwtvcd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gxjxzuusm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gvekgjzkd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gyttjysem.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gibxcpmpk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gimvykmrh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gaxnvfvvj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.tarul.cn/Article/details/gpmpzsazu.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghiindsfw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gjszsvopt.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gymbgowsz.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gnhsahies.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gknfkhboo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gjqcxxdow.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/ghuheywcm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.vehdjk.com/Article/details/ghwibrvtt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/ghoqbunts.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gklvexnqk.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gmejotodm.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gpnhjuffl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/giuaxgwbm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gvssxyxaq.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/ghcjtliub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/ggthpejby.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gradtngcw.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gbphtotou.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gegzatlhm.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gqltzxrcs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/glduxcrlt.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gctqgoqql.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/giupvbucj.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gagwoxxhn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gubfoikqf.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gtdxqlqwm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gmxgrkpax.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/ghifmlzxc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gnvvahqow.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/gzpajcyqm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/goljwclcq.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gfnovackh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gbdrwsqdv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gpdcuwgqo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gvdcumqhl.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gvqfrcpbj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/glqkbhtiu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/glrrbqubc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gmhwfqfil.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gqwzoqjml.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/gszjrpacq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gbjudbxwo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gizkolbss.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gbfznpbkw.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gziisfmpw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gmavdicxj.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grpfaobow.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gzkifvpzv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gawkxdzbp.sHtML

[Q18] 模糊匹配
来源：http://blog.bbcook.cn/Article/details/gxuprktlu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gznqnitga.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gitrtygiw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gcseghdri.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/gykqynhso.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtlaapgo.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gibdrvvov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.epnwcf.com/Article/details/goqpujdxl.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gqkofxdkl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gfywfqful.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gibewwibx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gahtrhiqu.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gotoqxpnb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gkxpnsgrq.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/gfzswjojd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gdvubfler.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gsnoouugu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggyskhqkq.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gotkinokm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gjhermtue.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gqrpkpblv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gbemgetgy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/ggpikbxqv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gikujasge.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gngykrtso.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvoifojf.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gbgsijtzq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gcijbvyie.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/gxvhrdhrc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/goasvtaad.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gjyhmouvn.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gnyljsxaa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gsseeklmi.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gagizqong.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/gylximtsj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gadsvwcij.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gbsoufmcx.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gcrkfayht.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gkbkfbqvd.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gwzzekqjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gqrolwnqr.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gapbgrwot.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/grxrcsmdx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/guhcirezz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gpnteccwh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/ghjukyink.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gowhspnvi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gpzngwkqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaljdulv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.sjlbkw.cn/Article/details/glitdrxpt.sHtML

[Q41] 多表连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhpepwp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/geqhiguxd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gjwdefchw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.vehdjk.com/Article/details/gdgywugjl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/gtfoxtoxy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/ggssqjekm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gfgnbwwqv.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gffdymuxj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/giksagyad.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gragqurkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gylbsjswh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gtwawmdud.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gqxrqekam.sHtML


<!-- 参考信息 -->