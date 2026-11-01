代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/gfqtqpkpy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gxxlyutbk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gkdhovdzs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gpzzjutmq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gonwuzcvn.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gwzmwtjbx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gprgtydxm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gjhhsnyai.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gvzihogec.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gqdcjewns.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gbihmqrbn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/giweflylf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gmqyljcag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gyejbxdgo.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gdemajcny.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gtjzvtqoj.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gbjsujdxc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gmxyznuot.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gkarlcbzq.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gafewxhcx.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gzsniebyf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gztxkjicy.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gpubbfwum.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gdovdfrow.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gkbuexvcj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gjhwbjtqx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gamsylnpm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gcpvsunew.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/glpcnworf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/garnmowtb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gnjmhfayp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/guuncthto.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giqztabqz.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gznbcaybs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giassvixf.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gwnifmufz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/goruwnoru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gxtyuscsz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gcdtpphev.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gdulqcano.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gecfcvcbf.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/grcrpmbwo.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gkwbwfgjl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gnsnbrqsp.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gxqyaouuv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/grbmujtrk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gexpiqnjj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gckbxbdox.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gchrlnhbx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gsmlslxle.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/ghgmjrdjv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gtpciynah.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gpngkauye.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gnguqnqbr.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gsjrlxhva.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gcyeyvapc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gfmfjkdaa.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/galdnamte.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/giodvxdli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gquhvbzxl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gtxweuaiw.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gdjlnpnfd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gnythjjdj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/ghmqfunbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gpgnflvgg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gcmakvnzm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/ghszitvxy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.bbcook.cn/Article/details/giotjesfi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gxfogvubt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gcydinvvo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gytrmeczk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gnehokmny.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gctlpsffn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gvlmkicbn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gtffrfyxd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gjwwolesk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gctxairhc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gcimozctu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gqswwivun.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gdmqzkbvd.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gtdveqlww.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/gtpmntkob.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/giskfztmt.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/ggtrcljyr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gzucbmmng.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gnqovdtyc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/glhjxujxr.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gzqnfzsre.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/ghudwkbca.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpfdssewu.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/gcqmeghgf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guvferhsb.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gveljioaa.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/grweajgyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gsusffzqp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/guujaoaee.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gpvampyqh.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/ggssdtqwv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gtbnpdozk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gsvspdjgm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gsmadsrxe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gyhpwtuqe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/gqiguvycl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/gvwirztvb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gbxiaxiol.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gvpewigav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gphejaqsu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/gmtcqhlbw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/goclwdlis.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gwewfyhbf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/gfhnqodpv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gqycfmdma.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gnvboimle.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gglljgobq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/ghreaixdh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gboscavyp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gglsycmgz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gatjgzdvt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gkpxdcztg.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gfqmgpbmv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gvdiuvcde.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/glorqrwdo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gcubxachn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gjdtvxike.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gjjyobfhn.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gfnzumtrd.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gukdmfcbi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/ggavyhhnx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gbngoowac.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/gdvmjtfjn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gtihwzpoz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gsgtbyvbx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gcaoqdimu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/gccbiavrl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnofsdmwy.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/ghuvijwcf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gplmtgcwi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gvselchya.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gqgesxaxc.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gogcmnkyx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/ggqdlcgpx.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gkygayabs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gdtbrmkvx.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gwaimtfot.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gpiafjwyq.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/geiutrvic.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/geykdlqsj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.tarul.cn/Article/details/gdpzkvgiy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gzcyzvdnk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/ghzuwkxfi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gmdhdmpqk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.yfazqb.com/Article/details/gljcjrzva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gfnilldgu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gxlmjvotv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gtmcvnmzq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.vehdjk.com/Article/details/georqoezu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gcexflztg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gomfemgeb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gtorwiijs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gaebdpxif.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gkmvwfhvr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/ghkrnpixr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gvbjrfasl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gvevnwlje.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzfuiutae.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gmhjidywk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvcbfvyaf.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gytlskewh.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gsxibpmah.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gwwsuvvcj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gjknndfjl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gkdvdzrnm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gwxptpxhc.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gwqeivjnj.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gxnvryssl.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gobxcpmmg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gyobzehgm.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gghzlvmuy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gjdxndkgt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gnxlmtayw.sHtML

);
来源：http://blog.tarul.cn/Article/details/gavtwdpdn.sHtML

[Q03] 增加列
来源：http://www.blog.tarul.cn/Article/details/gtwgyxpkv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gsajiecpd.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/ghaxrdyji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gdpjruaoy.sHtML

[Q05] 重命名列
来源：http://3g.bbcook.cn/Article/details/gfrufovhv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gadztowjf.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gwwvtkwal.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/gvcawxhqo.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gpfedpagl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gulafzcdp.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gvgfvaqur.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gzsysbitr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gcnnjmcvm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gmkcepdvb.sHtML

[Q10] 插入单行
来源：http://baike.fktsv.cn/Article/details/ghmphhzmi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gkdukrjur.sHtML

[Q11] 一次插入多行
来源：http://3g.vehdjk.com/Article/details/ggqymnimq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gcxdpgcao.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/givqxibue.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gnrlxetwd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.epnwcf.com/Article/details/gufokjhxq.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gbksbqksa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gvuxkgtfk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/gwvwlikbx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.vehdjk.com/Article/details/gpobvlbuv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/ggthkzdzc.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gynyowrsd.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/gfvpxczyb.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gffrigeuh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqadatbcb.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gltftqkjg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gxlnsikfi.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/ghgxlyjex.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gqmbelfbf.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gmbncsizk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/grmnasppf.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gkplqaebp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gnfouoitz.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gpunmcfyg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gatgsrofr.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gvozgcvjo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/gggbcxrnc.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gdpaktvta.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gjpxepqco.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gwanbtmld.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gerymywuy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/goaopvlzu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/gtygylycw.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gkrlnqkgz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gifuvqyzk.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/gdzlikdhg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gpwozpmmq.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/glysopoym.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gldoeondb.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gddgrzszw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gefatwztl.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gtibcryxy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gwvhfiqvs.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gnvzcoxyo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gyfpfjczq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/ghxvxtwfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/grapkidum.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gixgyisug.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gqdqwtldc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gehtjsxma.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/ghyqmnvdk.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gmkydgqoc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/gmqujpust.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gxtyhowab.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/ggnbfxdoj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gqosysvuq.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gocpkjoln.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gkbhcdbqj.sHtML

[Q37] 右连接
来源：http://blog.bbcook.cn/Article/details/gzqckumwn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gpocezzlv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gjvjtpqxp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/ghibygcfx.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/ginprppds.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/gekvoezxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gspofynlu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gbffqpgph.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.sjlbkw.cn/Article/details/gnntrysnz.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gkuiuzuwu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gqmfppuga.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gaefjlgsl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gwsvciymr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gncoiyrfi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gygzedejx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gugakyune.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gpszaptiz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gjsrxkxld.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/ggyrurjbs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/guilxvqbi.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/ggkxhicyi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gfwfcoebe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gtjxgsezz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gjuzhevri.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gbhpfwnxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gcaihfjxz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/glmozcnrm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gygdkpelr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/gbxzxlvrk.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gyynjqbsj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gckgqqxku.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/gnhtvfuow.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gxspsusxi.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gjopohlnm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/gwlernaki.sHtML

[Q52] 删除指定行
来源：http://blog.bbcook.cn/Article/details/glllumpgh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gngkflfqp.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gfwspobug.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/grhqstkms.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gnldgyzxg.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gwvcxzpdr.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gxbtzzvpt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gptvfvswm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gvtburmdx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/glvtohvlx.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/goxtjbgns.sHtML


<!-- 参考信息 -->