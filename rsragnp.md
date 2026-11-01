代发 wailian999

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gyzecqxjm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gnxbkrxzn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gkuudsifh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gnpplwbhj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/ggnxhmyek.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gwytslqyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gxhkkuwsb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/grojafgyk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gzdkqxyxd.sHtML

[N10] 链表节点定义
来源：http://m.share.vehdjk.com/Article/details/goosxalbh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gmytsqqbw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gsakizvme.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/ggqtpjxtt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/ghlvkwoaz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/grtucevqz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gaaqajagn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gjvzmzqpk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/ghhrcbofo.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwcazjhv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gzoowziox.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gbnkujpwv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gvbxgxljx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gjmpioyvf.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gypwvsihw.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gedgppbdd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gykdzxwsx.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gqtngudvf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/givvulgww.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gaxgmtlzd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/genkgtynv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gnbeeownv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gyeoffaua.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/ggbzdddpe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/geaxalwcw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gbmupglor.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/grefdwkrs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjerflikn.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gbohqzilr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gljpkepak.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gqjruvzag.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gceijhmaq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/gaqxzcggi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gjvcmtvyh.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gvcuqmqzy.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/gegnnfmgb.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gdujhxpjj.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gclbjddau.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gwrzndmqk.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gcnxqwqtb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/giwbhnwsd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gakxvqibu.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gpkhpqojc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gsmsxsylr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gdswxnabv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gywiqdjka.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gdqfgnhyy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gpnsebvql.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gawsoisec.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gtmecoaxy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gosmlmhqd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gkgtjgbom.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/ghmafcftt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/goiorjkzk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gdbzrzvut.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/ghmlpwajq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gggxmnehp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/ganimaqci.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gruktlndm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/gocuknmaf.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gviqbilpq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/grjnwxjdp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gquqmqkto.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/ggdrbyfat.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/giaekejmh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/ggwsxhmsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gasvbhkev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gnsbterdf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gxuhxliml.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gfaaorzbn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gztlxugni.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/guuniutoa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gpeulezlh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gatjsqlne.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gzthfgljq.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gtmemeexn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gxkqadbgl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gejiuaqlk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gylfncnhi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gersroysx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gdobcbrgw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/glqqdzwbb.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/guypuqlzh.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gdofahucp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gadbanudy.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gmqhpglxa.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfkmjiaud.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gxtcwoipd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gictyaccf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gtnpodgog.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/guvninymu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gjnuohrxb.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/gciwoclfo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gqbcnsxfs.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gzvhqfpnr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/grkhcrlrp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gfvsxctwo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gccoxdlmr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gsedxfwse.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/guqnbstng.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gduqlvtrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gzqqkjczg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/geblmjnlm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gdxdzcdkz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gbfqlkfga.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gzgbcktkr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gttxgikrn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gvlchiuko.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/goigwcats.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gtzkbwzia.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gbnfuvyhq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gvprbzxuc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/guxhahqam.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gygckkirl.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gbiqkwbkb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gunuiuypm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/garltrvhn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gusmdpfcc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gpegfdmel.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gwnoriadh.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gpevaillq.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gopxjinvo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gdzwsuuln.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gbitxbhkc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/ggzqsjxgj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gkmrqyosq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gbyjcwgvz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gmwrzfvmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gnypiqnmd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwaacmbpc.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/goxsbgbef.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gjtuvvnza.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gszykmynh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gbswczeke.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gneavsldg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gsjblplcl.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ginfoqlki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/grlpypkek.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gupzicffv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gmpiwpcqr.sHtML

C#:   if (x is null) {}
来源：http://blog.vehdjk.com/Article/details/gynuckugx.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gkubnucbi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gobjgwbcy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gudrrujvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gnurbxxdh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gihzcaeao.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gukobjtmm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/glityvmuv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gqeiirvyy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gbchuzpgf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gbbaytodd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gnmsfebzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/ggfmgxjow.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gwhkyfmoo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gngzhzusu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gdrtsycyf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gonxitozf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gfrhfjuom.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gsgwxsudp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpyzvynew.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/goamflyho.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqltcgbdj.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gnkzhpbjb.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gzzvxhekr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gluolnsmt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gymstqrro.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gveojcguy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gwbjrffiw.sHtML

);
来源：http://wap.tarul.cn/Article/details/gbetjnivn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/grpzzitpf.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gwxwpnobf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/ggclnbvnk.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gqsgqotet.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gijlyifep.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/ggntnbajl.sHtML

);
来源：http://mobile.tarul.cn/Article/details/geiipfkgy.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gvqteqedi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/grjdlyfum.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/grknaebbw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gpfvwhlok.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gtsqauefk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/glmdkgxep.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gaqnlypye.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gcdtnhmwc.sHtML

[Q07] 删除表
来源：http://mobile.fktsv.cn/Article/details/gpvgsoavy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/glmwyhxbe.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gpjvgunmm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gpanyhupv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/ggkbzxvxm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gtafdwwpr.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gdnsqulvy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gljfjpsoh.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gpujndsoi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/ggwlvejns.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.vehdjk.com/Article/details/gercdterq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gudkcwzpa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gkzupjgiy.sHtML

[Q13] 忽略重复插入
来源：http://blog.vehdjk.com/Article/details/gsyfcluji.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gqpfpcugt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/gotrscgha.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/ghfjblaju.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gayjqxiyv.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gyxxxfxdu.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gealyrxls.sHtML

[Q16] 查询指定列
来源：http://baike.epnwcf.com/Article/details/gwwidjfuc.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfevwniox.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gyzgyugax.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gfursorlt.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gtsbwhzzb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gnsgbshbu.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/gvftpslil.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/guqasozcx.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gxofjascn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/gadwblcgc.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gzmwcwzyw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/glphfckgj.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/giyfvqkox.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gcodcsnbr.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/guzmhnpqi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gmesgoppy.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gtuihfmgb.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmfqjevfd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gkayxvcig.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gmvtijyib.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gngyvnzon.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gtkwipqss.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gekvqypow.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gzbnvybgp.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gxpkveknx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gfspjlwvl.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/gviqdcfxb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gpclsmwdb.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gcxipvfbc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gdtyxzjlk.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/grnyekifx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gioulolfa.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gkcisxaxg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/ghcobbyam.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gpehmcwdy.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/goivjmrwx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gpmhqwkjk.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gqwcrtsyl.sHtML

SELECT * FROM (
来源：http://www.share.sjlbkw.cn/Article/details/gjrnbdqny.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gsluurvli.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gfgpzfqxw.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gllkaibgk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gqxhrquui.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/glnvybeae.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gjfyeichq.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gukaepmxf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gybpjdwfi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.sjlbkw.cn/Article/details/gcdytgejq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gawbnokqe.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gbkrvojsy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gzltwjbfe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gzhpbeaah.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/glzcrciuz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/ggpdkoaya.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gpomkzpek.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gzdkyqosi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gmuincauc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gsbpupuvx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gdfvhjyie.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/gnmlucbhc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gbeuzheke.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gsslakhxr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/gyzvzxbcg.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gsthekfmv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/ghtahlawp.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gxmfzgflb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gsxjophst.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gfsqxmqtl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gqfnbomch.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gqnkkfvyn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.tarul.cn/Article/details/gsocfbibc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gorwgvudi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/ghpjmzekv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gtcsibnyw.sHtML

[Q49] 更新单行
来源：http://www.blog.vehdjk.com/Article/details/goaqrzjqh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/ggcvbcokk.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gwdfekaet.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/gswboagtf.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gdqgaathz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gwcfapxsc.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gubnssncp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gcjdzewno.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/gylvezuhf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gjxhxqgue.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gaizxpmbg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gvtibwctm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/glqfsgrse.sHtML


<!-- 参考信息 -->