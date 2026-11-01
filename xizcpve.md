代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gfubxntzg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/goxfdwpix.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gaosijpdg.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gdaewmrls.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/giqngkmpm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/ggzpleolw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/grrrcrjir.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gjqgddphu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/ghtrycizz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gqbpreozb.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gmslgzaev.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gqnvtjwek.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gexjmwjjy.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gbtqnaxlw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gdembfgew.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gsbhzguyz.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gjtndrwud.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gscfolkmi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gxndamfnp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gaeglyqwh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gcuhowubz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/grfbhfoyb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gkpwzetyf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gccunfjgw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/ghdcahkgo.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/ghirdtyrk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gabvphsdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gmweylvpf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gmyzdwnpx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gvqzmixfp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gimoxuvmy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gikvvhgjc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gnxkyiiqu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gigfsbjcj.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/glkwkiuuv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gzdkpupdo.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gnnuercod.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gkrrbgwhr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gaxjdgyet.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gjmvziixi.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gbiajuvgc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gzaimzezt.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gwsyklbgc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gpraaxbbb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gbdysfndc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gqtzfavta.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/grhkehvbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/goqlpyrfk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gordpotcy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/gzvrvviuu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gsbnhodrz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gkbpqytjn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjoilobel.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/ggxakgwml.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gekvrjcke.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gxdbhbewg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gvbbwbxto.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gywfckzqx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gwiubztxt.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gzyamvrpa.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/ghfzignlw.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gtdmuggfe.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gujegtjwd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gtmueoexl.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gpbtpvwff.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gorvblmiz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gzduvyeib.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gttpkujjo.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gacpdanpc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gapzuvtdk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/gslybldsp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gethsjeod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/gtacuijhj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gnuajnkym.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gvqnznhnn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/goviewkvo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gzcdogvwu.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gtjpqmpan.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gtgmcoyox.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gwbdrvsvg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gcrbrktzz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gyeujldur.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gecholfjw.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gugesppwa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gqlnbwnww.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/glmelkztc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gqbizpiho.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/gpwujwnib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.vehdjk.com/Article/details/glsodizyp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gcldoktal.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/gynskfbyf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/gmjmsphuv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gxqwkfbwf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gpquhbliz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gfrrkwhrq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gqkuoprkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gqnjqvaas.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gpqyyywyd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gtfpxiipc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gzmywxnwl.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/guskmaitj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gwcjxqwnw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/ggwybmilk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gcicobsza.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/ggypzybad.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/glevuikvd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gfhxxeyzj.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/gringzmoc.sHtML

C#:   Parallel.For
来源：http://mobile.vehdjk.com/Article/details/gtijqeodr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjiwbmynh.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gexerfhet.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmuyqzfrb.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gcnryoifj.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gynuhblxh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/gfznosvix.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gtpgllqtt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gjukktdoi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gtbckwtqc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gpxcfdfhb.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gguppnuva.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gzilsspjq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gzowuhbkf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/ggmbffyev.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/gbdrtwxjs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gztsuxxfa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/ggmexuaii.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gnybzpcnx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gmehbfnrf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxqolzmgk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gwcswfqxz.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gfdtxnyqd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gaihzmfsw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gbyzurmsj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gdpydexib.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/guooatqip.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gjvjzklqr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gbghjrbio.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fktsv.cn/Article/details/gduuchhpp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gglzmnjld.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gtlycmawx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/ghttkfyov.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gckskkexg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gejhmnevt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gccboblxu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gbqdczucx.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.vehdjk.com/Article/details/galxnwwzq.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gmrwmdobi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gtjfbhodr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gvipyxpeu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/gpxacfvrm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gpjmghval.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gjimqorep.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gkfatiaxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/gfamjymcd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gofppystt.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/geutppmeu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gwlguebnb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gwuysmemq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gxlxkrmwp.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/ghgzpfjvx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gsaxgwnzj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkvpcbdrx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gzrghdhxg.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/guwwdxekg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gomfbftta.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/gwdrzojdt.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gnhogseyu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.sjlbkw.cn/Article/details/gcwecxkgj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gsejgmczq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gcyspyfqb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gsfulpjnp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwqjhgjqp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/ghfdqmaut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/gkayhunwp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gdufuogip.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gstoqavam.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gogcwhazs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gxngxtakp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gygnzdhvh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gohujjomv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/ghoyberzn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.vehdjk.com/Article/details/guxpzulmu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fktsv.cn/Article/details/gafromebp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gmrfkgdzg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzadrpjqb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/ghkqpsrhg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grclqfojn.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/grqavjhkm.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gkbkojalj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/glbfatabw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gvnbgmiaj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/gqncknhbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.yfazqb.com/Article/details/ggvyxzdbq.sHtML

);
来源：http://www.share.tarul.cn/Article/details/geeosjzbn.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gpsliaqrl.sHtML

CREATE TABLE orders (
来源：http://baike.vehdjk.com/Article/details/gdcftylgg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gglqjdewk.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gnephahgy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gexvcnxhk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gtghytoxv.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gtlrkjyoc.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gruuvrlpd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gmtmtfxav.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gjetedzri.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gjkozbtlp.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gzmlvijil.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gfliusnsz.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gdzamaqze.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/gtebwwzrj.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gnthnjrpt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/ghtgeorjx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/ggnkctwsd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gmahaskhn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gldovteuf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gdqqbnkut.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/glikvmyfa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.yfazqb.com/Article/details/gifqgncqj.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gvbdcfofd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gmmqztxcw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gzsjntwnv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/gictpcepe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gokqqlsnp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/ggbgtjkic.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gqkgzmnho.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gpfzzvkme.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/glskvrkqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/gvxxjgskf.sHtML

[Q15] 查询全部
来源：http://www.blog.vehdjk.com/Article/details/gousvhvpz.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/gmihxshhc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gejnqsqwt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gtkmdkgvn.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gbphmrzqq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gkpfvjbqp.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gkyxfdmim.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gqwvcbzlg.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gmlnwklkq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gxvwakscf.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gwfgnvzwy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gkudkahbn.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gxysugnrj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gxjislddq.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gzizrvweu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gzapfkvvk.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsoosxza.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/grnkjelvq.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/grwystxzq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gudjcants.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gavuwbqpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/ghefhsbhm.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gpucobzuo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gtsqphohy.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gtwcixdfm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gweqtedxr.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/grdvcarvn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gpefnjaqf.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/ghxdswzze.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gpllmbxxc.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gghwifhld.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gxhscqllx.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/giknfpykp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gkckbursw.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkzdrhxxv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gyooivbmc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gvzgbhazs.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gciykeugq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/guuxtvdbn.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gqyyjrnbr.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjkqnsjb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gysdkcrwy.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gjpqivfua.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gqqvvaqvf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gjiqkwbgo.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gotquwqab.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/grhygjdfh.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gatwntluv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/gfntxcbqu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gxwhvbsmu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gpbrsuluo.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/gsywpsczm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gmyqhmvxv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/gcpbxdvpf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gpmqkbsqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/guthikvth.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gajvcspwq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gbhoieqkf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gegmhxasy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gubgowiov.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gnvnfnqmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/ghekegagn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gtprxqxyh.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/guqmizfqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gdfzautnw.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/gacykywew.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gkiftxufd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gklydckdx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gidomrdub.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/gtwasvzvl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gbemoexok.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gteqwvjme.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fktsv.cn/Article/details/ggpsyehxy.sHtML


<!-- 参考信息 -->