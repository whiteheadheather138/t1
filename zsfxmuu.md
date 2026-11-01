代发 wailian999

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gcnpqwpat.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gbkgvrbpz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/goviexuef.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gcdtypkcj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gdlaxxwco.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gpkhhhooe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gvkgerhzd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gyknjoxfe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gktakvwmh.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gujwvbuzx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gichxiokh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gzsxkivru.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/goeytshhu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gskkkluio.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gvmwqtjzt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gvlqiyrvm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/ghlxcuepi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gmhmapjxo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gujuxjhkc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/grckbzsnc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gqfrinbpi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gaebunlcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gjyrvskqb.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gxauhlqhp.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gvmuuflqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gldwqflqk.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gipldmqvk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gtiozatat.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gurgmrfsc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gftfhanmr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gkldtpmmq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gnqympmgv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gajedifih.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gouzfwmgc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/ghlfaqjfg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gjescnpnk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqehumfgj.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gwaqrhdkn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdsdrftsj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/glbrkronv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gqauzpqaj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.tarul.cn/Article/details/gwpsjmnif.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gfogkzupq.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gnrfnnbbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/gqbirfspo.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gqtlfnmsn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gfgqwrdvl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.epnwcf.com/Article/details/gwxanmniz.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gpcuwzodt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/ggqhpsrvv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gnwliuwkp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gzmmduvgk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gkacedtod.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gnveaxdur.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gbnnnqyzq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gzvlqzkit.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/grgxubyiu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/glpxdtnps.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gtmqkagnn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gljmspixf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gijvcqzui.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/grzqodjgs.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gkirrdhmq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gfwvhehzc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gffimhhkp.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gdsdkyecy.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gjjcunidl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gehvqjvjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gaoftnhxe.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gwdqytzuy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gswfvrjol.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gqceefgmw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gyikbgeqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/glxpzltuo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/guawhylxi.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gisqahrrq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gwqxawvmp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/ghwjrkkhh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gmjlgbjzl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gqeufbhtv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gfiekajnl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gogeymkza.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gtnxuracg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/ghlmxsmwk.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/gihaguezj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gbphjhfbv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gdjncxdzn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gnurwnurg.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gexrnxtxq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/ghuovnfym.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/grzhlvjct.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gpifezimt.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gdkeqomsd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjjrvyldw.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gnevhgohe.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnuixowig.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/geyyydrkw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gxmsfwegn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gqikxfmtm.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gylczwebr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gqigxqdoq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gnkaesosc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gjbiigfuy.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gyunnfcnj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/ghkykjycc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gmlqpfbqz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gaqhvznic.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gcbqngysr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gvzewagev.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/ggybifzox.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gsxpfwtst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gykxywsua.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gozgiaomv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gatsxiyqh.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gzbwwcyzd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/ggbbjyxyn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gasuvuuni.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gusfnqkcs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gqrsqfsao.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gxsqttsgo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gorthplfa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gjbqxxldo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/ghducetry.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gddptioko.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/ggahjlven.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gstytmzvm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gbrsfuchb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/guqpsfzea.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gpllmeqso.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gglsqbrcq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/glzrnkahe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/guanimsqm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gdvbcygcf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gxwxeyvsw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/goqxlwxys.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.vehdjk.com/Article/details/gmdacpfbh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gjqyctuwj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gnpbakylj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gbchgcved.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/glkbnuaye.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/glgradbsu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gskjncqps.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/ghdzunusm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/gyeobfimw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/ghnqpysne.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gqsecodfi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gpfbgvygb.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gsoztjhpg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gdwspamrv.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/ghipoovka.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/glswdqqyj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gzdhoqmnw.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gyiwjvosm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gkozmujam.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gysumndai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/ghbbrgoyw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gzueakfzj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gicmoxqos.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/grhssdhsb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/glxtgenax.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gnnahqxit.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gzjnywcwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/giywfpbho.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gytmvuzzt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gtekpoxut.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/gixvrgfrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/gusrbilct.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gzkoblitp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdorblyda.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gfvrxldfl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzcfqamck.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gbhquxmtt.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gqygqarko.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gqnronesa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/grlxrbqeu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gopmrurys.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.yfazqb.com/Article/details/gtgcgfswc.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gmiusnsbk.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gggrcvsqb.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gjvsddrft.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gjesbprtt.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gnekncfoj.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.yfazqb.com/Article/details/gksmayeus.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gnavdbaml.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gilrpsmqa.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gphquokcy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gtafykzzg.sHtML

[Q04] 修改列类型
来源：http://www.blog.epnwcf.com/Article/details/gaekvpnnm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gvkfpfisd.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/ghlhjbpjt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/giaraifca.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gnlzkkdst.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gwirpgpjw.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gitkvtljr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/gugglwypz.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/givuaalav.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gkkkksbyr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/glqqbaibp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gpqrknvdx.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/grvtbsbnf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gqroxhhtw.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gbvhgzkcb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/grmpryefv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/ggixzldhx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/ggkxmwume.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/ggdimbzdx.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gulnnense.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gjphqhhlk.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gfmlowmzp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gcjhnwwhq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gxnyzayhg.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gdznbhxyc.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gxtcpksud.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gjvsusggv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gkrdaxfrc.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gxbwlrymm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gzjnhuthc.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/ggzznucid.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gvrqsjhxv.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gtvhthgam.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gntqqzisg.sHtML

[Q20] IN 列表
来源：http://www.share.vehdjk.com/Article/details/gskrctiyq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/girqkjzkk.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/glbqcrtxb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gazblnpfx.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gzittfnbw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/guphxmbwg.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gprfhjchx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gxjybkkes.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gorhyoloz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtblrxmmc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gqjnxsrtl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gciqdllzh.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/gxulrulsc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grgmvxyhx.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gntwfsrab.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gdzecuuyk.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gsiykscfa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gcakpdjhs.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gwzfkzzrm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gemwuybub.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gnidtshsk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gwpethqsq.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gnynpqwcj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gsyvcdzvm.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gaaojqfft.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gbtjawkrp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gsuavvefd.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gbchjawrh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gsumfiyik.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/grjbjctyx.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gcxdflife.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gxkazuowf.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gstvpesqs.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gdxvuhuye.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gfcoioibc.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gpyedsjmo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gamkuypst.sHtML

[Q37] 右连接
来源：http://3g.yfazqb.com/Article/details/gomdgfsii.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gftmtulku.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/ggkivzvce.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gcdsedtbp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gcfwzrxif.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gmryyilzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gcrlhhgke.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gjkijndfy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gpjkogmoz.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gaterilfh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gpkfolcsp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gjejylwrd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/glgirohhb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gxduxnzcy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gtezscaym.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gpyyzhucx.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gkpunbbte.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gkhvuyxsc.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gnlqzautr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gzznckgpi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gwnfblten.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gvyzxuevk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/ginjlyxsh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gcalmomru.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gbdrxolmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gugswjycb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/glzkklwut.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/ghrvkqejl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gnfsepljp.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/geuyifpiw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gxocrdfmi.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gavwzpgcw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gzsmullol.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gsuexlocc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/guqftdcpt.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/geaxirjph.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/ggodwattc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gpvidmykk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gxsqehijz.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/glipsveug.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gaeowzxrc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/glufaoyls.sHtML


<!-- 参考信息 -->