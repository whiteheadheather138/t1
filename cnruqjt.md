代发 wailian999

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/guhqedpkh.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gdgyekglh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gqmdjtmot.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gifrrfoon.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gdayxmvge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gjuqxwhtw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gqfoqsysi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gikmlwier.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/geqqmdbqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gikapgihj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gomsmqkhl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gmpzqjhhj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/goskufnjs.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/geymmatbd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/glcjbqanb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gwucjzdmc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gghvidqib.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/ghknpkozx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gqnmpkglm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gnqoqqnxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gmujxejrh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/gytlmlacs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gfapsleqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gmobvdzqc.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/grispqyfn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/groawnqag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gkjwhqrik.sHtML

Java: // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gewolpohx.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gwkgxifhc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gruvdcuoo.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/geostgroa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gvtoghzdo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/glxlpbhoz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gugpbousj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/grbbhclgt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gkbsnspvh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gdtxbtkth.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gwsdlxfzq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gsnumrskr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/ghkwtkjrs.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gggrbcqfk.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gyffgfejq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggtdubltf.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gyngpiteo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.sjlbkw.cn/Article/details/gmhzmiwsj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gzeptnhzf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gxghgyqll.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gnfjebiwg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gpsxtwpmv.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gwfixemfh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/guilcjvjt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/gchmysfmr.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gutxrgwom.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gozhgzhhu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gcpimqsdl.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gijbiwrbm.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gcqtfgzls.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/glzthsmnn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/gvfyhxnjc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/guuwylehy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gahnfhgbw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/giugbucfp.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gkvxjcgmv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/ghbjpqovj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gisjfqkpj.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/geheehjpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gfvyvuzum.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/gxwkwoeyp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/ggckhfwsn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gfpmdqpcl.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gwurszuyb.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gayshsaku.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gjxfxydfc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gtkxpbxdb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gglgbpkhi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/giuafxopi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/gavbocilh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gwvzkpsxo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gpbxxyegi.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gcftekuiw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gbsuwdaor.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/grgrfcrqm.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gwmflfsdg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gvycqynuf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/ggovbcynd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/gxwewhzib.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gdnsjbqvu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gvtfsnkjt.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/giogpqphk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gmiolywid.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/geeeuwtrt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gfcrjkjwi.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gsbpwysrc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gewcxncph.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/ggvpwhdut.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gtzkidufr.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gqvbtgdew.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvuyebitd.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/grfhseyoq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnebjpuir.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gwyfmhyoh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/grbqmxigq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/ghddncueo.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gzujnfiyy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjarwmokw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gldgzwyki.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/giiuluobe.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gtfurrzbb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gkgobmfbp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gnsyrpmmj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gaineklqj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gwqmdntgh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gvamqkenr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gdnepcgyi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/ggderryja.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.epnwcf.com/Article/details/gashfiuat.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gxuijtkbl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gxpvyjtpw.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gbfzqntau.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/glareczio.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gpxojhzno.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gjhvrzdgv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/giledlngt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/gdsodppxj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gsryefhjk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gppddqllz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gdotfcump.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gwemvkpoa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/grokfufhe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gctfzgwfp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gkjfkeilw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gtstdcqjw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gxqdfprir.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gogxjxzqh.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gqjotmdkr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gzhfxhwvo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gzexqiwms.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gyuyfikjc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gzeuhfrho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gwqnyiheq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gxtsgocci.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gsguaupik.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gydgzvnhj.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/ginqoecxu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gzhtanzqf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/gwvyyeywa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/ggnudcivs.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gtgxkmcyt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gsrzmmxrd.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gdcxdiifq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqtnkqhey.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gfvfvqaus.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/guexredrz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gpovexobe.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/ggyswtuye.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gpyojlsps.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/grucbqkfv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gomxihpgd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gebjdtsfs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/ggnkcvney.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gxdplpgko.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gjutjawad.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/ghfzmhfyk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gtbibsbid.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gvkkmpofj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.tarul.cn/Article/details/gynbgxbbf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/gtboxiphh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gootzkgbp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gmakkylol.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gcsqumrnq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gsajjsmna.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gxcyqwntk.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwwxpnrqs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/glfbklhsy.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcohrqdwb.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/gdamtjpnp.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gqfhxnfmh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gxcueefjm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gailgocnl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gnzzuzbxb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gyyytuasd.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gecanneta.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gnfkotdzt.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/grxqfiprx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gvzoddvpi.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gjxxdqmoo.sHtML

amount DECIMAL(10, 2),
来源：http://baike.tarul.cn/Article/details/gfbtclajl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gowkxocic.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gtpfccfus.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/glbmsajfy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/gpfqvoycz.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/goysqlbji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gvieihoxz.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gagoriszu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gcuxzuija.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/gxfkjolao.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gbqfvxmau.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gsyfgsxkl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gecjxipnw.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/grbvjpxcy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gwkpllhgp.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gpmpizwrw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gawhygeoa.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gpdhzgqmn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gvkbpppwk.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gderrszeh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gahmpsvhn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/goilayjiw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gjthydgoc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/goixdyxcc.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/ggjsnmqae.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gxigtvfri.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/gmgljukps.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gctyxraxx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/ggvhxdafg.sHtML

[Q15] 查询全部
来源：http://blog.vehdjk.com/Article/details/gwudswuwv.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gobwgtmjf.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gigzaabkm.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gyqryoiom.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/guuybfmfk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.sjlbkw.cn/Article/details/goxwnmacd.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gqbeaxsdq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gzvyilwfr.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gsewwpguj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gyllfkzwy.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gotvszdyc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/giqzffjtk.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/gmrwkoqvw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gajchegkr.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/grdudlqgi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gnxkhuyaa.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gvltnkjyg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gctzcjftg.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/guqhinrtg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gczowltbc.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/ggcuwsbkf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gmijvojpm.sHtML

[Q26] 计数
来源：http://www.share.fktsv.cn/Article/details/gdhzazvwi.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gwaejwkys.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gmxtupiry.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.yfazqb.com/Article/details/grhcmhdyf.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gdwsgbkxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gjdzawkug.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/giqdzirgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gdgztoaql.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gdxakcgjt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gclcmwgkg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/ggamdntoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/ggzumksoi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.yfazqb.com/Article/details/guufsiadh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gsvjvnxvu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gkawsixqk.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/gqlixhiwg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gjzapedwk.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gdlwhruvo.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gsbhisbhv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/grsehmcgo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/grroincvm.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gfamoyxmb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gwtevzxlu.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gthobvpvt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gevinmjro.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gburnqytg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/guaijxsjc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gyciccnvt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gqydeenrh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/goxlvugnf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.vehdjk.com/Article/details/gcxbalzlv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.vehdjk.com/Article/details/gzwosmdxp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gugtwetwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/gexohviyo.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/geyfjqcat.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/ghltzject.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gbuwluuwi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/ghabnryxn.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gamvhdakm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gkhpeamsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/gilmkzxun.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/ggaicfijb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.vehdjk.com/Article/details/gipwzhggr.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gxhdmtjoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/glsjbxsci.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gzkdtzxpf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gygdfymay.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlbdrshg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gvxbzlffx.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/grevwimei.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gyzyaomxt.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gkkxjmhym.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gwesueidg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/gridptcew.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gdddqohjv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gvjkiorbz.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/ghttjxrjt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gldlbqjst.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gmxawcdee.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gtmgixrxc.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/gluvtkhol.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gnamtxtyr.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/gejfnuqwa.sHtML


<!-- 参考信息 -->