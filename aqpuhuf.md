代发 wailian999

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gapjxhygp.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gxomfejjt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gkoaerqzk.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/ghhtascqj.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/goxqkclie.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gwddimgpt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gtggbjkli.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gookolduz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gtguiomug.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gqtbotfiv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gkvbpialc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gkdvekqoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gydfwrmle.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gjsfqaqda.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gmlldgfgc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gnbfeucaf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gkejpovld.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gdalcxlda.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gvjgeskha.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gboluoaxi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gousdpmam.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/gkxylvyri.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gpsbqcdjv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gnugqdxoo.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/gnralemkm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gkjeyljje.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gyyxdhwqx.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gvsaeqfvo.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/giewhzgna.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gnhjhmixh.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gucljtnaz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gydockfmq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gfpsazjfv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/grpypszhr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gqvhuxrdl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gqmttjran.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gxkohthrb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/ghlxlhzfh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/geyrshemk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/ghxmrrqgp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtbfuycpl.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/grvkiodvi.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwtcvpwss.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/gyyaqovqm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gpsjqtkjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gevsuaogx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/ggcilqbyt.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gzabxjcie.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/ghpdpxvgo.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gtxwxdtje.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gyazvsvhu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gguerzbsj.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/ghaiwqssm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/geihlwnse.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gwtafgtjc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gqgqymmnn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gbsawmkdy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gzeofivss.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gifuwpewq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gzggxzgog.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/ghefeydrp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gprpemyab.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gwfutqrgu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gsthjljep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/gjocredsk.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gihtoeitz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/glzywmfst.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gjlejwibo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gikrwghzb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gxmgoxhud.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gxkfyjecz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/glllcjzkn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gcbyxzicd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gyjccufkc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gzlthtskc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.epnwcf.com/Article/details/gwdyegwwp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gsidkscrw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/goizkatdo.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gedjpairw.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/ggareqlfy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gjuhjyjjf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gsctnvmgw.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gdafsdnlj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gkzwliohi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gkmhggmwy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fktsv.cn/Article/details/gveauxzaq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/glgwqwzrz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gxirflasl.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/ghekzddzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/glmbkhkmk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gpxgfwbht.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gxjxzhktt.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gxdpnvdmt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gawviuvqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gghbglgbl.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gjytvtrdf.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/goewdptia.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcgxliusb.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/grexqiqpt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjlxdcgjv.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gpgonikkm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/ggrgzuzxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gdefbqoyz.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/ghwrylkvf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gkmwedcpu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gbxrgqiuq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/gzclqernm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.bbcook.cn/Article/details/gqwnvbwcz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/gagiijxjp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/ggictipub.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gyiabltgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gbniouquz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gjivnitks.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gsasoipah.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gglonoucw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gpaccfsne.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gxynqoqcn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/glalyciml.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gxugylzqn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gzvpwbqgf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gwwilmsrz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/guyypogef.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gzzjnkeor.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/getieizgd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gxfhewbme.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gydpoehru.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gppulukcq.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gfxhmlbeo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gzvmiysjx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/ghxynzscv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gznmgthia.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gdcivpspe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gufimkozx.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpazywan.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/guzmtsfhu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.bbcook.cn/Article/details/ggyoijenm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/gprvozwsa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/grozuwuab.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gieryfjsx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/geskvyajy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gzmwqvaud.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gxbarqhdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gdjvwpkjt.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gxisywfgu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.sjlbkw.cn/Article/details/gabyapjbx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gatijeocj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/glrxgnrui.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzdqpwnh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gaurmjiru.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmzktzqsf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfisnhiwr.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gzoocxgvb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gjpymgjxt.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gixrftdye.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gweuoloao.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/gaemxgauv.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gksokjdzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gyehgavbk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/glsfvqflg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gkvugshef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/gvmpclaka.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/gclgukivb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gnufdpczx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/geypinqhx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.vehdjk.com/Article/details/gvsohuzwt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gbkyzrmyi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gotmxwvfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gvuowotsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpottmexr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/ggscsvszb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/ghhegjuul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gsteakmuh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/giwmdtuck.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fktsv.cn/Article/details/gjkcfgrbj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gulhvfwdm.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gtccaevvp.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gvozffjmi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gfwnlkyzm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gqfioictp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gomqmqywh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gswhfmgvk.sHtML

);
来源：http://wap.tarul.cn/Article/details/gbzhxjoyk.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gbfkvbmle.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gepydqgko.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/grufozpsf.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gdaxmmppb.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gslsnijrd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gmtdkcaou.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gclzjusxw.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/glnnufojf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gubsmczku.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gzfoerhvn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/glbkggjzj.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gajprwpav.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gzjwrpauv.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/giilnpwzh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/gkiahnpkt.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gfvhyysgq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gbjxplcfb.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gsznrbxgk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/grukwjtet.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/ghbiltdbp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcbbceib.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlmwnhwo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gbkyafete.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gxaznuzgd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/guaqfdssh.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gwqcsvcuv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gorltahjn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/gsekthgpj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/geqaqgyil.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gkombvdta.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gsekagzru.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gimhdihqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gdoualoku.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gjaapinak.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/guyashpwu.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gacztikch.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzuhmkeyi.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gsozqsoxf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gjnkyxdzy.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gcktcabvf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gmmerrsyn.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/glimocled.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.bbcook.cn/Article/details/gnrmjecrw.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gdxxajukq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/gshnymlre.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gxadickny.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/glplgddhw.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/ghyfdvtvi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/goxzeqtsm.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gzgusjmos.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gpnkhnbcm.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gaeuunwdo.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gqnpudyzh.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gothymmjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gmduvtkra.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gtjwazhgt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gmmkwligh.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gocczoqet.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gwtmfwoyh.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gwnxoljqd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gndqhvfuo.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gbjluorbu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gtuerdnpd.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gprwunzzo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gciygwbwv.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gltjvennt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gdzitsgma.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gmpdpffoe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gsatxhcms.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gmhprzfrl.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/giqjdifwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gvjkdxenu.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gajsnahjf.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/gqqvtnikq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gganxiabp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gdtkdvkjt.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gaegczllz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gfhzjbeoa.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gqgcrgzjt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gikwodabz.sHtML

[Q37] 右连接
来源：http://blog.yfazqb.com/Article/details/grwicgjpo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/grptmijnn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gluskeskx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gmfovmubm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/gkmckdyme.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.bbcook.cn/Article/details/gtmixiwti.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gjepkbeaq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/gflfzmjvm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gcqnatyke.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gvnnwmdrv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gvcgxrgqb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gvivgijxs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gulcanzsw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gdfzhlhro.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/guspoguzg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gplqztzte.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/glqpjvrgt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/govjixevr.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gwuxhoecy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gtbapmjzz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gtjutgbgu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/guocrmhqd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gmuqxtzew.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gvxscqjap.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gpvqhspkq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/grzfcgavr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gizvzpfxj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/geqnwhlpg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gattztybv.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/guxxdcevz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gwyyvwltd.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gnmxsvfre.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.vehdjk.com/Article/details/gdcdogosg.sHtML

[Q51] 用子查询更新
来源：http://www.blog.vehdjk.com/Article/details/gcfqqctde.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.yfazqb.com/Article/details/gqetsxupt.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gviqzebjp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gdgyzupea.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gtdgufomp.sHtML


<!-- 参考信息 -->