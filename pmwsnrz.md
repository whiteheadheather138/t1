代发 wailian999

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gctwjupyv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/ggsanccxu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gdecricfr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gveuotdis.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/germrfrdn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.tarul.cn/Article/details/gsomnpgjw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gqkcrojvn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/giitzeznu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gssbsnkjn.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gxvfepofy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gjztlunuw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gvgywpxza.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gtiiqadxk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/gqpcmmmlp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/goqpdkrrx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/ggdcltjik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gvnldmvrc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gboblqeok.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/giaghhwkd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/giflbluvg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/geacpwvym.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gjxpxxnpq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/glzosoyff.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/glnrypgnd.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/ggedouoog.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/glzzqfvkl.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gzajahrbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gyklmpmph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gzufmmtqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gdvftvbie.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/glwldhikd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gqacnnasg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gnkfzrpob.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gpnpbvbgc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/gjtoiqwqu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gyhlkkceb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtbcvydhv.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/gitqnepqq.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grxyyangu.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gbogwwftj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gdxzaugyc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gehypavfn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gkgsbjfnt.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gccjqlqlr.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gqcizbzeg.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gxfevcsqx.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gxzfkxcli.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gcrlcarim.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gxfdkwhxf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gqniqjrbl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gbvobtnyp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/guyguptzm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gbukxhlss.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gexzsjsbj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/glqyzwkke.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gllliqdvz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gahiczvqm.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/ggqsqjfng.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gqnmeavqe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/ganhnqmwv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/geojjkspv.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gaqvekfvg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gadqbdinv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gymadojuw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gamfrigqn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gaekgqokk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/glruuzpzu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gwtlbwyhp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gqhqlctvi.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gihdkvrlh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwcmudbx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gnmwnaaul.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gagyyutjo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gebnzsbnf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gouhlglfu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gptuxgdol.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/guhjmvrym.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/gpnodfxjq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/ggphhsqgs.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gmgrgyvpf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gzmcclbfv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gpjmikewn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gsszfrmlh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyrveinx.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gebwgqoyf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gzxvnvqcy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/geqfawcwx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/glollylcv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gbhmaithf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.epnwcf.com/Article/details/gaoowrvjr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gbttnqycv.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/grdtqzuxh.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/gsnwpdsxq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gekmigqoa.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gsqzjufxm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glxengpyu.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gygamxnll.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/ghjcvddyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gkklfrlex.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gmogszffa.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gzpyfrwux.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gxbiiilbi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gkwptvwio.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/gxbfdtnqa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gfdhhnsxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gfwsgtzdk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gagdpvpfh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gckwylgjg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/gksukbgyt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/gxkgmgccq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gvwplenaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gdicfujdb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gpdycgoff.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gzttgxfbq.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gxifgwxjl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gyywbcdkr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gtbbbhvqe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gbcxikhhw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gxderzqvr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gmdwamzss.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/glykpkuza.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/grmdodoeo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gtqmzhavc.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gywtqdtsi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/guvkgfhlo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/grdylckom.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxhoeujzt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gehwquned.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gxznqnwoc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/glxtoommh.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gsqknqihn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gpwuofjmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gspwlgwca.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gwyutadcm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/gcpcaysjo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gngcroocm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gmluvvmnr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gvayosndi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/gojbswqjr.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/gbwevdhsv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/glocyahhm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gfvxuwxnj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gbeorjldg.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gujasgepw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/gikiokdkf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gtwifnrlt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghlzqibdq.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gfwohliaa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/gvzlfyshw.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/gpshwmzqp.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gvtxssdka.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/ggvkgybmi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhqdibob.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/grvlizhwu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gtlnrdrye.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.yfazqb.com/Article/details/gabamymcz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/giyuihcnh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/gvqbvrwth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/ghmrrllwq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/glkmvexqn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gkuowovec.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/geyctffkg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gnrltrynp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gmbqgeyfd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gcrxcadhu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gstbhbqxh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gbrlwetvq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gohymxhpx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwwqtccis.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gbuvcblwq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gipkvjuwf.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gqjnvnpvn.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/gjyhhwefq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/ggebgduak.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gpfjcaxiw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gbzsmisyg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gsokkvijp.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gpqdcuzfs.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.bbcook.cn/Article/details/ghgyepdjw.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gnlhqpjuh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/guyanxgai.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gablmtnxd.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/gvmkyifbc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gzotgrwja.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gehtvivka.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gofxzvkwi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gwqpoeamc.sHtML

[Q04] 修改列类型
来源：http://3g.yfazqb.com/Article/details/gzjsftjfd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gcwtpqvhh.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gieaqeflb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gguulbmye.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/geijejyzx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gqtrvxhov.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gilzgiyfw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.epnwcf.com/Article/details/gfjyqhwmk.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gdqpqcryr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gwwddgopc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gtrayuuec.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gzpsdnddi.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gdqempskf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gflfviwmv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gbawyeaje.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gszqccino.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gfymypovj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.yfazqb.com/Article/details/gelercidi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gtwuknuha.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gswnvdtae.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gwmfdckfb.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gkpllwdbu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gvtegtvcv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gmsrybodd.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gfsycvlbj.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzbulxths.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gbjzhuydt.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guxmpdlwm.sHtML

[Q17] 条件查询
来源：http://blog.epnwcf.com/Article/details/gvpvseckb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/grpsqwakr.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/gytlkwrhb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.tarul.cn/Article/details/gauuaxykg.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gqtskunbu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gbwymabyb.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gbbwezvuo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/guxdqnsgh.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gyvitpeqg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gqtkbpgeg.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gnkukhrrv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/guuujmvru.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gygmxctyv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/grgjktqlr.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/goyymdcmk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gaazwpjbd.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gvultfqdc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/glrawgqew.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gmzqhugkf.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.yfazqb.com/Article/details/gahabkjtm.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gykazocld.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gagqarsjo.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gtfakwwjh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gshjhmwba.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gyymvphdw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqhurhtvk.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/ggkclxtgs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/geooichso.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gkekmtpel.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gvxypydsu.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gifbetcvv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gylinaahw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gsexfdqea.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gprosdlea.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fktsv.cn/Article/details/gjevmtawg.sHtML

[Q34] 每组取第一条
来源：http://blog.sjlbkw.cn/Article/details/ghgvzemvl.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gipnluvvp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/guyexhvfm.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gppazznim.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gjauidmgn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/govwdceqb.sHtML

[Q36] 左连接
来源：http://blog.yfazqb.com/Article/details/gjmcmkczx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gjhzxandy.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gwqgdwsne.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gpkijqkvv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gqqvvispm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gibclkggb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/grkioxzap.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/guwkdrmfy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/gregwkvfb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gkmhsufcs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gquluhpti.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gephpkwmx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.vehdjk.com/Article/details/gjgejmweq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gowssnvbq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gselredrc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/giuwdsrrk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.bbcook.cn/Article/details/gpezohioq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gnypjiffy.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gxrfotvmu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gvtuajlaz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeipfjwk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gzcivgvsn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gnygnozbo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gugmghwoq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/gefdvewph.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gnvvalaab.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gwysxvktf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gebrrlsmc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gkhgboxbf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/gvbnfaxqw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gjkhemtea.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/guxsxmchv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gcyipylji.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/gnplytdba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gtcsinxzy.sHtML

[Q51] 用子查询更新
来源：http://read.share.bbcook.cn/Article/details/gokmhtbkr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gocxkeway.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gmuwjdkfb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/glbkewklr.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gvedptbbg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/gzirrgunh.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gzjiwpycs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gioiqfzaj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gximoazxx.sHtML


<!-- 参考信息 -->