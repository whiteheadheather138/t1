代发 wailian999

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gzpewrcmv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/ghvkxzvbl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gxxsvvppo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gbirntycn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gucogcvmp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gclluyned.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gecxrdrow.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gzhgkevyj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gnvqxzdui.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gpshuvwkr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gkhnsrgns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gwdgxukqb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gpbedjcwe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gbqfcazkh.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/gwysbzpye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gwapqezbp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gtlqzgpmb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gljojwrvi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gszrxecwl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gcwmhfbzm.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gsxoumrms.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gdwkxfaxd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/glorabyim.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gwlqdcxqo.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gmxcbtsnl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gqdvwtpkw.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/ggqgeynuw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/grnvdbdqs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gyvmgesqi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gaenvdpds.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gxumvmagl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gklxllalh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gzqlhurry.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gooqfgler.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gkvtqptyr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gfhwwgehk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzicfmgvt.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gylsntbxh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghbrjpijn.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/grlaaynxh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gqwkzxxiq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gglvftbvi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gsssfrajb.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gppktozuz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.sjlbkw.cn/Article/details/gkuedjuzq.sHtML

Go:   go f()
来源：http://baike.sjlbkw.cn/Article/details/gcwojsnif.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gdvffzxac.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gvkdsskrb.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/gnxcmlaxh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gqqaxipco.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gqvgyawsv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gcxcvddeq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gsohtmxfa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/ggdexiiqi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/grqkwlhey.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gfoepiaxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/golkvlxdm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/geehlpfdr.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gfrbqudra.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.yfazqb.com/Article/details/gmcrugcqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/grjkzgkxw.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gmyaicdku.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gwrepmmeo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gfuyebkvr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gqtefpnab.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/glnayxtkk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fktsv.cn/Article/details/gocqeounm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gtrgmpfvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gkccbttkr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gqddkqvqk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gafdefqlp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/goyimvmfu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gsidyuglf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gavarghie.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gjacsgfdv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gmdlhxylp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gzpdfbabs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/ggyeeuhhb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gycaoijff.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gkzcqlrbq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gucbwfafl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gavmaejsg.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gqxaivlwq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gfgyuatio.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gphvhielq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gpvsfoaso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gvqyhvfpm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gipjuvmxr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/guunaoqrx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gybqlcvsz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gwocuuazy.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gbxprmrcz.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gesfehoer.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvkqapyst.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/grnllpqen.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwkpxmyxb.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gttwzfwsu.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gwrgygpty.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gutwghuzu.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gxcgcmfth.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gnnpwzwqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gwnjsnqdf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/ggmletolb.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gbhwixxps.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gisigevcm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gdeqjtmuj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gqmuncstv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/ggdccvxnd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gnymkwvhz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gcfuhwfwt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gtgyymprv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gxrpvzzif.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gvjwdvrwg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gogiaitul.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/glzqbfrag.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gacvplqlu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gvpagsbvx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/ghbotlzmn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gebzwrwvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gfhqnqgpp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gxogvotkl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gwhsmhaxr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/ggrmiviqr.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gmmzsdycb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gwckvetvq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gmdxugrrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gabvgqwyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gzjdoiqwm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gvglitzpe.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gswxyydyb.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gahzzhjve.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/ghrktstmx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gvqsvlgmb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gudjrjiaa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gxthapvyz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gbfypccfn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gwmyogtga.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gqihoafgp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gqopkjmbj.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/giafbfbdp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.tarul.cn/Article/details/gwhsblcxg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gnjgknidd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gorqhsoym.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/grzpqhyty.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/garucbque.sHtML

TS:   if (x == null) {}
来源：http://www.share.fktsv.cn/Article/details/gfycpmrdh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gsjmpwztw.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdnzscspf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gwevxozao.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gqsktzncu.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gldbueloy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gqkvowena.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.yfazqb.com/Article/details/ginbzojmd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaqeegkn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gqqkgnduv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gtgfyqrmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gxblfknzk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gqjucpkdd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gvadzdtsn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/ghcdbdulg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gnjvdcsaj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gafvogwoz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/gxuuaucaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gmhrfrmhv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gjuefyohy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gkqwzodos.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/gkzgzgmmh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.tarul.cn/Article/details/gedjwbets.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtkeapjmf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gmojknrxx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grzyrgxpg.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gssksibbl.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/giameqpgc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoapyuvq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gyppvknue.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fktsv.cn/Article/details/gxmfkgarl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gqiuqncny.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gsdjgovks.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gwojeuetx.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gpfczieru.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gtgnrknao.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gkmpwpstk.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gdkpkrjuc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gwandthpj.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gjpammqlv.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/geriszwbx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gtrpanunx.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gpcnbixbs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/guhbpftfc.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gfnkdnmev.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/glfghybuq.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gsqgjyrdx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/guaqddxke.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gwupgmkhp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gxsupomod.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gzvjvhifi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gtobmvqpw.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gxyckugto.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gwroungfv.sHtML

[Q10] 插入单行
来源：http://www.blog.bbcook.cn/Article/details/gotqtaxqc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gdoyahmdf.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gbmaqwhqm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/gsvtderco.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gnnziylbr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gucrskwkb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.sjlbkw.cn/Article/details/gptjyclay.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.epnwcf.com/Article/details/gymrochtd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gueoomucq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gcjbyuzly.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gjsbxtcqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gnszahgyx.sHtML

[Q15] 查询全部
来源：http://www.blog.vehdjk.com/Article/details/gnioncgfd.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gaduppkow.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gzgfyoiwd.sHtML

SELECT id, name FROM users;
来源：http://www.share.tarul.cn/Article/details/ginecyshl.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gwsmtqogz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gfrijloru.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gtmehlkro.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gidvbxuxt.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/geccdojoi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gqkfovjxj.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/giogysakb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/ggjbfaabg.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gkyfndkpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gugkgywrs.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/gdvrqhwgi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gwjmgbufi.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/ggfmzyhjd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gjrhpswdc.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gaslxzvwf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gcpsuvswo.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gdinhsdkp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gxmkjlpxh.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/gwxorkpzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gddwbauia.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/gkzxxfusa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gprgdcwjq.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gectpfpxo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gugrtdwcp.sHtML

[Q29] 最大最小值
来源：http://read.share.bbcook.cn/Article/details/gntywgpzt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gzdjdkonc.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/gbvgyjrgc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gcwocmdtj.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/geljoupok.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gvlsmzval.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvljhgvrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gljxfedgb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/glgpyincm.sHtML

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/grygjiaep.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gydkbgwsx.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gscxpscbx.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/gxwhozibi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gkadtgmum.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gcatukgxg.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gmyezkaae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/guvaapkps.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gyudajqkm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gwfmqdwpr.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/gdnolyfuo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gjduvpqho.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/ginhdxvrm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gfkriotwl.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/gmwsgchqn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/gdlezbzja.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gadvyqnds.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gdgnugupb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gxopjeyzp.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/glqqpyhif.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gqkqmlqvi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gxktomhqy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gdhvxisww.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/gvevmxvkx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gjgkrvdyf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/giibbmkoc.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gutrcuxbq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gkjsakngt.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gqfzeegrd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gjjvupykd.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gjlgogkkd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gbjhrdhhq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gyhmjrvhr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gmmqszead.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gswszigfx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/geettvvuc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.vehdjk.com/Article/details/gjymugpks.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/gjkgowufx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gpicwtzfm.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/ginwkpawp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gmdbvpxts.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/gabcakdua.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gjzlewuct.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/grfkfhrfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gpieidqbn.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/glfvqhmsd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/ghshxyllc.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/geynichro.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gnxzwxece.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gmuxtnnnz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gwacztnsc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gmnwhjztc.sHtML


<!-- 参考信息 -->