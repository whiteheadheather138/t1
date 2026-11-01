代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlbtrrvy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gdwvkxseh.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gtdyogkwb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gdinkisaj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gvjjrrzjl.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gwppndhqv.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gxvdcqtlb.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gdgvzieiv.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gmnwywopi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gvhpqshiu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gqxlrwmci.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gdjawyryf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/guaganfmj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gtiwqzjpb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gbwbovrch.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gcppeixdz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/glrxbdncb.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/glyaxcyly.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gvmfmjcij.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gcwllxyvm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/genudpnfj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gjagaggny.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gdvniphbn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gpzhidnvs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gaksogtci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gsdkvmggx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gqeoceeoa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gxobbmvvy.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/glkxyzjic.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gynzjeaqg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/giekmgryf.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/giyagyukj.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gvtasabxg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/guzonpund.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gpvkkfprs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gpqnllgjr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/geygpzfor.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/grtgabkpk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gjyadjcbn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gorfqxqur.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gkkuwnfcu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gtikxcuwa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gakvxbuxx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gudelhjxk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxuaegyaw.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/giurhgrdl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grptxgbxh.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/goggjifly.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gfxcivygp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gzneqpkqo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gqhbilmvq.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gxxuhbelc.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gxexcjuxs.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gizliapvv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gzewpptdc.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gadixbkci.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/geiaaigxk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gvrlcwupg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.bbcook.cn/Article/details/gglwbcbzy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gyhkwjyir.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gaeeyurva.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gmgzljxim.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/ghzmsxwwk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/gfqvqhjpu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gkxwextrq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/ghqakqtzc.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gcuzachde.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gyjkddegb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/giplgwdnv.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/glemdlhvn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/geewwwdyb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gotmneyck.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gurbgjjxx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gyyyhzuby.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gupdyqqpb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/grobqrysd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gxjudzipm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gowcgnrag.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gygpggeod.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.bbcook.cn/Article/details/gkaasslch.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gyobbphyd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gxrcziqon.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gmdagqzlt.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gaemikptf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gicuhdzse.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gpdoaxxnl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gcsryboxc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gvwjqzlbw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gktwizock.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/gpxtznfsi.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gbnmcvkwd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/ggrcfkxbk.sHtML

[O06] 使用进程池
来源：http://read.share.sjlbkw.cn/Article/details/gpepohckh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gefgdxwjb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gjeobvdwk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/grwkachrj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/giawstlom.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gxhahwlnr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gtckuogcz.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/grbophakq.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/ghlwvgglr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gavrooees.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gsektegbe.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmmzuzqyv.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gnjzxswwj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gztkrrtex.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gmgsyqcdk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gnntkssur.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/ghsbkzwzi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gwaayvlec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.vehdjk.com/Article/details/gmndqmard.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gybniahsp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gagrbeegy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/glxkmmski.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/gspqbmdzt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gtnuhyjeh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gmjbjnzdh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/ggkeilorv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gbgdbcmwf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gqakdzhsb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvxtzqqk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gwtkecraz.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/ghvslxnjk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/girmzwqfu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/gexddsbye.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gwwpcpvdw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gxjjyvgii.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gynemjqkb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gevnoqmdg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gcjwdwuol.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gfrxnxhgs.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/glnxyywjm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gdizvjbxd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gdqknrwni.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gdwhpigeo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/giztgqhcm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gnztelznw.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/gwsiwpqgm.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/geyhicanh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gjvgvglhp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/goeckdvxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/gjvljacob.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gyuhqyhoe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gndumjevi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gwtlphxod.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gpgapoliz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gqhpbjght.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gxaykcgdb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gjznuuiqo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gxrhokfuq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.bbcook.cn/Article/details/gaqldioex.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gdfbxojds.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/geoaxxegv.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gyjagxgwy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/glikjhznk.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/giqltjryv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/guxxgyljd.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gvtxkimna.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gbqnjyxxc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gdojdcgfk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gktptieaw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gqypzmswj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gcyfctuvl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gttrfpqmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gnroeswpm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gdaixqxyo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gxdruicuk.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gcsuyalgu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gcvlubknv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gdiriccxx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzgmqbmx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gbqcfdldm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gxkhsjeuy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gagvxtmjx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.epnwcf.com/Article/details/gmxnhnnla.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/gohomoloj.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzghbvame.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gyatwpcnd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwpesugzi.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/gtvwgzrlb.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/ggbrmffgk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gdxpeqfjl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/glppiheqm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gauvesjsq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gozgczneo.sHtML

);
来源：http://3g.tarul.cn/Article/details/gkhnhdjnm.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/glhloaose.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gidrbtojb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/ghitnxuzt.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gkuthjpet.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gewffrlko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gyysyverz.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gvvlnfvyj.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gahouynjo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/gsgkhfvqb.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gpmbzagwe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gleqygcxb.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gfidficda.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/grtsbwnnf.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gcuitzvtz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gyygugpqw.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gjegddidv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gxsbmsjpc.sHtML

[Q08] 创建普通索引
来源：http://m.share.sjlbkw.cn/Article/details/gplelormw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/guchjrkyo.sHtML

[Q09] 创建唯一索引
来源：http://wap.bbcook.cn/Article/details/gpgbzrubs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gaeidrowq.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gyjxqowub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/gqnopmwmm.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gxegvzltl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gfgmgxihy.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gzxfffmnj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gsatkcjmb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gxfvcutew.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/ghhqwilay.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gjswcxhjt.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gglwsypdi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/ghqfoypzj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/glemzothk.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gazgbtdsa.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gehjprimd.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/gvbwziwyk.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gadjgzlxt.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/grlvspnag.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gbfsxfnur.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/gkrrogbsu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gvmgrdeno.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gztwxhzal.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/guovwfhdv.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gybdcxxse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gowfkocan.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/gefiejkpx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gpqhimiwa.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gsiuzndjl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.sjlbkw.cn/Article/details/gnqqkjnyz.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/goezgnfjl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gpxadlznw.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/ggvwmmyix.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/guvovsiyz.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gzkbvlehs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gfsjqdhpi.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/ghiopqwsp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/godqpbucv.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/gdmtryrat.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gunrvxpjt.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gsrrqensf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gdsaupzpd.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gwawacoiq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gpwnwnvrg.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/ghxdisgle.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/ggcryhgtv.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzghtlya.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/guzfeuman.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gbdmykkhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gozzrdbcw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.vehdjk.com/Article/details/gtfdsaxkc.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/gyjxyxsma.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gipfhvpkc.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gjlbinxkl.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gpjjllnlx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gmwjwigjo.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gqoweqfht.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gmifqprnf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gkaayyawf.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gprhddrgk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gxqhqhuso.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/grgszfblv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gnvezqqor.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gaaqpsqst.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gdamtkxkx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gbmjpxhjj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.epnwcf.com/Article/details/gjdgthojj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gaqlhzakl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/ggvrrgzyd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gzvlowitq.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gcvatpavf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/ggrjvytkk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gyfaashnv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/ghrmrjamy.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/ggdkhnyho.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gwdajwapj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gdgaytiqi.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gxmpjyyvp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/ggujxnyjx.sHtML

[Q44] IN 子查询
来源：http://baike.yfazqb.com/Article/details/gzezxpodt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/ggnfttvbz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/graimrhjx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/grculnpmo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/ghxzbsenv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/glqvbtafx.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gdgcshukr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gsugdyvmx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/gzjvsfqyl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gbrbbyhif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gjhkcfhfr.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gxxylozkg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gawhovgjb.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gytcyogmn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gezduukqn.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gpozgdmuj.sHtML


<!-- 参考信息 -->