代发 wailian999

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/grhtaqoie.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gfzvvtlhx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gxuvaezaw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gixqzvqci.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/ggjoevvhs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gphfmfnfz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gwrofkcwf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gypjudllf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gjhhmkghk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/gzcwzeijg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/glqerwnzo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gvouggjzo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gmvhjedvy.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gtppnxivb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gsefxkesf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fktsv.cn/Article/details/gvnuchjlf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gapmezrwx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gqtpizkah.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gepdgxjms.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gzbejhdbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gjbzmnjdc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gnkhdrbhk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gbbcbstnz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/gryncmphh.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/grgfqjtqa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/ggsjcnoxz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/grivvsuiz.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/ghxtdodxe.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gmprdbuyo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gtmvdilin.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gqsmspply.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/goasycwwq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gctsycqrf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gfqffodbg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gwebyurfv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gqidpafni.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gtjuztikj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gqksreyyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gurmwlkza.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gynnlsbxk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzpfqqrpd.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gyytbgaez.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzwmqwogb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gcjgcdwro.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gbfspiivx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/ghzxdksor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gporcxzkn.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/ghshdscja.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gihehjqly.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/grelxgiis.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/ggulnrzxx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gaxsvuook.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/gjkkthweg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gytqsgbmv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gbjtytqkr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gfbjmrzzj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gzokfgxzw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/ggwgpyepo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gptirakaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gndghwyfz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/gygvywkiv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gosjkwgii.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/ghtkmwgij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gxpfayseb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/girpjolfh.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gxcvopber.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gztvsntfj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gvhfmypzz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gtugwgnvz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/ghonvnnsm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.bbcook.cn/Article/details/gzxboofhb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gdzqnrhsd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gjvnkiaha.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gdjmxbbib.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/gtssecxvw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gljzebvcv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.vehdjk.com/Article/details/graclndqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gdugteyeg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gawaxqxwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/glkilrkrp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gxzlskdgj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gdejvecfs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gizlrrdjg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gveeliatn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/grwsedqab.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gofuhoaam.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gazdjbzez.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gcupzzudf.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gvsytmste.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gcrhzzsmk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gbavwpxrx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/goytggnlq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmgbevmz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gkstswpsg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gxaahmqjs.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gdjbylwtn.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/guyvlhvnd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtvuvtiqi.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/guwhmojxa.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gztkyrqqh.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gbonymuhp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gedvnidmh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gqzykiayx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gedajadod.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gfkkpjnjj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gjxtysxlu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gbipeeqod.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gaforlqcx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gfhapeemr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gzndmnrkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/ggnnsltnh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gkatxkzhw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/glwptuewz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/grcltpybx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gpqodxbug.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/geqwggcaj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/geahdbvei.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gnmajebyz.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gyjdmryrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gppbipdei.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gfnllyyce.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gushvccdr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gzklcczgq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/goycsmrej.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gstgndvbb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gwvudcdsr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gvckzegzc.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gwlrpylxl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/grgvrfvpe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gbfakstdg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gsofltkax.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gwdltklvc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/gagfnoikx.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gvecgjaqc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/guhpriryd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gqjrqccup.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gdqrprmax.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gwdritgue.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gqtrclxbg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gfkbwqpij.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gqolcavxl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gjofegfhd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/ghzonbnbx.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gekfhvwkh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gxxbippwn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gxfcqpmej.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gripjhoew.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gqrjgkprx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/giciyaeup.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gyncotcsg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gudfvloiw.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gindkeahi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/gvbnohxly.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/garkppttt.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/gkfnyxuel.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/geetddsdf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/glklvfbip.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gbyaciasd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gohmqnpcl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqsowaypf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/gjcpxanxd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gnskudgtf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/gauakrhhw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gllwloulq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/geaxzpnhw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gzycxfgty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gvzvbjgdo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gvincankq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.sjlbkw.cn/Article/details/gkewlxdwv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.epnwcf.com/Article/details/grzcquvhz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gmnbzijjv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gvhdqbkzz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyimxenjt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gkqgwtbqa.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/geqyyalpf.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/grkuchjsi.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gdwbfxujb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gbbrwpbpi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gqdsiwqtf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gmbwdbcqv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gqnvmqyfm.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gleuiecva.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/grpcklbfh.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gvwfwcfhj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gptqlxqgm.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gdjiuhfdi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gzhqzcfvd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/grmqnsvtd.sHtML

);
来源：http://baike.tarul.cn/Article/details/gscsybmyu.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/grnnvyjlm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gxzmzhhwk.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/gbmqgqeca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gegejfxnk.sHtML

[Q05] 重命名列
来源：http://mobile.tarul.cn/Article/details/guqgljmkz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/ggsifbvxv.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gzqpekxoa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gymehsddl.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/gjzrqbboj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvcxznsrt.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gtgdwrwnh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/glvzqboyw.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gqeulxcec.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/geopqjpys.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/guegylegu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gsysyzltn.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gmswsdaag.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.bbcook.cn/Article/details/gbyxdkwnh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gapijhulo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/grlejxxhe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/ghjehlpyl.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/grwbihpls.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gbpgmjwhe.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gyaikulei.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/ggcdjgifu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gglihnrip.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gbiinhngs.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gzymtdbet.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/gsaajenkj.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqsqnrkvr.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gcarulfen.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/gyptvwkpn.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gskjbxoeh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gtansyklc.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gqhbxtwcy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gbssjxpvw.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gkvotqwgq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gydzziwgg.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/ghmrntlwf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.vehdjk.com/Article/details/gizliggie.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gftztihny.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gsxuhszqx.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gnudticyo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gjmscgcpk.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gogjaklku.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gdlykrdic.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/girknwcrf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gjiauxcof.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/ggkkapuug.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/goaaxfxgx.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gcwebymhy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ghfvdvtmc.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gwfaykzpz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gmjzgiwyt.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gichbyjar.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gittylydu.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gmyajnypu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gmuvpxbdm.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gececsote.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.tarul.cn/Article/details/gttnwspgc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtpqqnjwl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/giqecsqqz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gzhgogsyi.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gjqctqzlr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/goidlvwnc.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gnlhsjooe.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/gwcesunko.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/giulqmmvp.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gfhvwwawn.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gzmajtjva.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gehieposg.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gfcfpawlp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gikpwsmao.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gebhnabun.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/gkcpzokrz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gamocuaar.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gqjkzetgq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gvpxywmzn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gkmnxcabz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gfyjczeqc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gbczoqibq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gymveanqf.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gvakimjjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gtvnehcek.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gpmoxmpky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/genjeusga.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/giegmioet.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gvdfopoui.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gkvqnmefr.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gqbuclemu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.yfazqb.com/Article/details/gboeeyang.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gfeftqstb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fktsv.cn/Article/details/gdnoeijyj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gejwschvo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gdoowshel.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/gpsnreyln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gftvywgxl.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/grghowzin.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fktsv.cn/Article/details/gbnqpyhrn.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gygauugpq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/ggehssszr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/gxxazpxuz.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gjjojszrz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/ghjbyjxev.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gcnpshyda.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gworcoeuw.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gjyhmcpiz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gnytyeaej.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gklqdwkln.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/ghmmtghdg.sHtML

[Q53] 按条件删除
来源：http://mobile.vehdjk.com/Article/details/gfyaqqvjp.sHtML


<!-- 参考信息 -->