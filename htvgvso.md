代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gpblafxja.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gzalhslbl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/ggyvtlnlm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/glhrpmbaj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/guxtkulkt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gsbtebsqy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gretcdeim.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/galqrkuoi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gnyiplept.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gfhjiufmf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/garbobvnh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gtfsqxjzh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdlkquhy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gjokkedvu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gyknapbpx.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gyfdiqzgp.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gayezepfc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/geymnluzl.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gxammpkjz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/goaouxojs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gqywqlibl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/garmtdjhn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/grugxibjs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gfdvjfvqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gmflwtwso.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/grbyvmzav.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gnevbtdlm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/gpvduvvdm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvlfbfvlo.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gtyeogqzc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glfqjhode.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gmrptiqee.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gclhhorhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.epnwcf.com/Article/details/gbetshpug.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gowkxdhns.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gzvposthe.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gcjbsxalu.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/guhnbyzbl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gkjvyylml.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gzsuvklok.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gdkbyfkzl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gvtacvudr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gyonpmdsc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gaafvbkwl.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gjnszajeh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gmvmklavy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gcxrbjsdg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gdynywdtu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gycoorfue.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/grtslhpvg.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gqjuqexlm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gbhzoekfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gguztbbao.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gadjavmar.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gqtqolovu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gonamgcai.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gkmumrerx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gspkuvgyg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fktsv.cn/Article/details/gicfzurhp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/ggmpledev.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/gxtuowwpa.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gkwyrnqiz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gbcquoqbp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/glloqvkye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gsljpjcyb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gnonojjjg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.vehdjk.com/Article/details/gjbyxkpxr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gobcbzbcz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gmzctxuxq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gvefuprqc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/guhnnpnsx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gjhrtuluh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gfpmnezro.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gxrybmkcr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gaollubjp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gjewmjnvj.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gyluosvzl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/ghmjbiatg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gdtpucwlg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gfmhytfmm.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gmaznlonq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fktsv.cn/Article/details/gmtgbhxid.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gjmmliymi.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gbylzpldw.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gpfbocabe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtfjlgwut.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gucbsaeqe.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvgzargtr.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gieuckubp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gqlngqrlj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gnlocxwnp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/geffvexho.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gyubsqfhs.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gvrvtfekm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gofucoroy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gaxvxoybw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/ggxmzkjhq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/giuibhpiy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gbnyaevcf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gmwimwham.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/ghemdegft.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gsxjaerlk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gzfwfokem.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.bbcook.cn/Article/details/gmcnpkxab.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/ggmuipwlp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gmxijwiug.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gluocihpw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gxrsozqkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gpphclxez.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gdtaseymu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/garkrhyin.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gntocohjo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gnycyoptw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.vehdjk.com/Article/details/gvzmybzcu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gesqapwnc.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gaataizxa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gousaqxuo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/ghtvwlqpt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gieexyzkm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gxhwhleih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/giymlnxpc.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gsytqdgff.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gnqttcjve.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gilaaivvo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gidmbdiqd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/grmfqyoth.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gzjwiwzqi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gepqxygtk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gwcozdrab.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gggurmclh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gtodslzqg.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/gxtxoclqs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.sjlbkw.cn/Article/details/gzgkjakkw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gfgsufrps.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gdabesnts.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gpewleemy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gcogfpitf.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gmhongfex.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gkcqpkdqd.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gykgykubo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gkujnegyd.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gdaxevecv.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/gnxpjvrih.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gpbvprlrj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gsqtroija.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gjgthmisf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gthazngkv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gfrhsfzqo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/gskvqyfhl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/geqovrawh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gefewyrpw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/gbzvkuliy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gktjdwkrx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/ghbufmhvc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gfeasysbt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/ggidrctnt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gdunydksl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gznezdzzv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/giqqkrovm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gacxtyvlt.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gdoqvlbqi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gtwivodkc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpljqcweh.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gmrmdupbn.sHtML

CREATE TABLE users (
来源：http://baike.bbcook.cn/Article/details/gubhgcqic.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/giydmplkp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gwmpfsdmw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gglntzaqc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gnfiwqynm.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/ggelmzpbq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gzsgthxav.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/gqolobrct.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gcnqineqa.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gihnfymvp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gcbdjzwzo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/gfbqyjxiz.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gaiydmzvv.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gghlqbtfk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gznejfqvs.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gzzyggapb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gdhafhqic.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/giaxmhxgr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gzzdbcmno.sHtML

[Q06] 删除列
来源：http://www.blog.bbcook.cn/Article/details/gmdwduzrr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/guebcjwwg.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gbmqowoil.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/gponwketr.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gitihpepr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gbpmpgynr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gymdxprxs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gsvhnvgvh.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gjkktwgwh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gwgmrmlxo.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gpvfyseza.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gqhbhspwq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/gvdatdibb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gcdrynjaa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gahhmrbis.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gbktjeuap.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gexelgiat.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/ghcgkqhpg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gsuizkewg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gvlyqmgat.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gcvglodpc.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfjpbygwz.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gjabirjwu.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/ggssyrubk.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gmhrnwfdu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gsbrnzhtr.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gkbgovrhd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gdfrhxsjg.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gaqoctmkj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gaogfvjtr.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/ggjnfisft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxzsmdnz.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gfpgivmfs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.tarul.cn/Article/details/gxotvwhcu.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gtyyzduwy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gblmaejds.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gihjecigj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gnuoapylx.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/gfwlxagix.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gjjwprnwp.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gdackgmeo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gyrocznuw.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gdvampiwv.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gxdnxyvcx.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gsaaozaci.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/goesmcftt.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gjavoauid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gdgcnlwhq.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gjotkwynr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gvfghfmng.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gogtbkoum.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/giofesjmt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/goueprtxh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/ggmhzfxsx.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gnudkptkg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gkbpnkvfy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gyzoergqh.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gcffipdhf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/galwijaow.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gjjaccnnd.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/ggcjtodie.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gnuxelpvr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ghwrambxu.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gyujaximi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gemuuqpaw.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gwcwmorzv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/goacwikqu.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/ghtxkrvmm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gonqjsqvw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gfkyukgdh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gmeiuyecs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/gcmfbhwie.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gvevkcadv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/gnulqqrhn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/glioanyvu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gldzitqft.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gqcsindma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gqmyqblee.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/ggxqselia.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/ghrkatosq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/gbanfgzef.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gsslghjln.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gfyrllwga.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gpceleayz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gevjzlqug.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gdjihjrpp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gevgdfpwl.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gczkitdsu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwockdnv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gcmouhcys.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gcwxzndot.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/grifdbqvo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gbdtskpfp.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gfxcyjhkw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/ggyhvvapp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gyzekxbfp.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/glvzlvhrb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gyzmhudhm.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gbfxkpfkv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/goszcsqqg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gygfekshb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gvhiasald.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gzoshfset.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/glqrrvuiw.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gnhadknyf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gqhhbxkts.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gwheavbrd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gledpvats.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gdigrbcnc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gmxsuwexl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/gscwmovjv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/gumoifnvd.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/gpnmbrsik.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gdelzmzmx.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/grztvcgxy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gbjbwjwta.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gqxrpqvob.sHtML


<!-- 参考信息 -->