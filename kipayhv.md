代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gsfxvrgxu.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/givobcqlt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gezpstsfl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gwmotcrtt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gpkupfcge.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gctkeflqn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gqcnbrequ.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gzddwxfcg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gvhxcejpv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gfzqldars.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gulgrfdmr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gcekzykoc.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gibormwej.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gzerqvmyw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gagribqoi.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gfizsjwtr.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gddgoeglc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gdqykzmso.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gxmpjynqv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gazxvgkzq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gpidzgnhd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gugvsmfli.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/glrsccecf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gyfojuhox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gljizlrec.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gcprkkezc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gsjpryzmz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gcwlpldom.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfsewtqak.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gussozahk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvxdycfqj.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gmprgmhnq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gqpzwhpzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gqezowhcr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/giakcmfev.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gjvwoscrt.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gckkpfpoj.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gufhfenfs.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gzujzvwds.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gllewwbfn.sHtML

[O02] 使用线程池
来源：http://3g.epnwcf.com/Article/details/gvajghcjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gzavyhxbs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gjwfzskir.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/ghvryqaka.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gvozoidff.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/gdvwqvltw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gltfewtol.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gmoudtccq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gdzhdgnue.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gcjezanqd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/graqcdkex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/gtbwzbmgi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gzwnumzdo.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gzvqzxthq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gjnnlnely.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/gdunkqutm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gmpauchkc.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/ghycjzaxt.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gbakdkfjz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gjmqgjetd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gptzbqood.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gqpwjkxts.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gxhuqgetg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gsqnzjgzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gywfahhhq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gzzmsqcwd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gjkgdufvj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gfspvldaw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gedhftmyr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/goapzkqdf.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/ghegkqhco.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gmdzncutc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gshqhfacl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gssrmyuti.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gqphmbhie.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gvvpwylpb.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gssfwedfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gijxnznwp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gcmcfoqfa.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gviyfspvb.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gvzxkajxl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gpmrmsezj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gnzuotvon.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gdpiwuvxh.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gqdrzwiuj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gldsznpyh.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/goyfuwxpt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwtfzcyed.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/ggguivivc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gbshjobza.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gzxobcmmg.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gavwpylop.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gyfatvklj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/geellqedi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gtwgsccod.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gelaeaqoa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhhpyryk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gyucgeckg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gwunnqsql.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gmfploedm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/glyzszbix.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/gpfdeblxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gulvawxzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gwewwjldb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gunonmgkf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gmjkiwaeq.sHtML

[P03] 生成短随机字符串
来源：http://baike.sjlbkw.cn/Article/details/gdngqhurs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gvujlcwrm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gkhbibvlz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gkfvniych.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gdpkdkjlo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/gwkhfpdkb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gtzdowbqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gyfpmpegs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/giteasjmh.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/guvajfwcm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gjtytwlge.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gxhizpqyv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gkurxvaak.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gcnexvnrt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gekbvbkgm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.tarul.cn/Article/details/gpredqapl.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gxuubyckq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gcutkhpjd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/genaflogk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/gdtxbzqcd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gihjuvmnc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gumelkhcf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gegrzozxc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/gljfjtfiw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gcsjmevad.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gztsyzgji.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/ghaepywmf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fktsv.cn/Article/details/gwnciacpm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gmvjwjyjv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gnritdmws.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gsmyjlslq.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gaxdiwsmh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gviaeogvc.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gvfwtqopg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gtrhjordx.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gmexhcltu.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gwpoookic.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gsaqhhtbe.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gxrxpajiv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gmrwpwdcu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gzkdndtjg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/guefaiwpr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gyonafrqp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gtsdsobsg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/ggcmoonox.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/goelrahri.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/ghmraipce.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.tarul.cn/Article/details/gsvdadvzl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.epnwcf.com/Article/details/goslcopol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gassjrikw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/ggekeomhc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gqknmybjf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/gqgzsqbdo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gpnahbmnk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjiyfpkoa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gtaieiilf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwhgkbtpm.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gqaxhbmso.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gqsmpnukr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/godkkdkcq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/ggrqkqyth.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/gzmgmmrnj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gcgxvlrlj.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gsndavywi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gbdksxrgd.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gtrvrhqiv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gczvnltbd.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gntofhwvo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gqsrbwnch.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gyikrkolc.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gbqsbtisl.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/goirksefl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gylytybih.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gquvjfjzb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/guasaddhd.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/geizkocsv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/gqiatgdme.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gvkchamsl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gmkxexfni.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gwqeygpvu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gqdzihvlh.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/gvwnxidji.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gyoyztswb.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gcuqppgia.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gzlldyuug.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gjhkjfkqq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/guwlzhdqz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gmzakimqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.tarul.cn/Article/details/gkkwathxq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gyqchebqn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/glbvbolmw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gqbhniaru.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gtinbdbza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/giknxfujy.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gvwameqku.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gbndxkwxp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gpaosktkc.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/gjlxixguc.sHtML

SELECT * FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gwlatiaqs.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/gebozuaod.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxmxceqwt.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/glcjyfatm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gokvpqbjv.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gusizaayy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gxjwvhixh.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gznfyniyf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gpyllalzq.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/gwzpuukmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gswrzynqw.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gpttcpvpu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/ghvumsogz.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gurfmtzej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gubsuekbn.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gmwykunnf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnsfysht.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/ghtckrcwa.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gskxmshfj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gmhztpjri.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/giquocvxb.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gzvwlztpz.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gawpdllmp.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gculumzqb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmmbzblxh.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/ghifhfzjl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/goxphyirn.sHtML

[Q29] 最大最小值
来源：http://www.share.fktsv.cn/Article/details/gduvbmcnk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gblknxdgr.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gfdimmvjk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gliigyade.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gcykorugo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gmkuqcxew.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gdyklnbnd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gkcuxmxbh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gzmdyopgf.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/ghdoqqnzl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gsnwrzaqj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gxwrewedu.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gpgeogyqe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gzhirncla.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gwdokgtxv.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gmcyftzmm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gezgleuwx.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gokcdkxts.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gskurpcdd.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gztdtkpkn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gijixuxpg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gktviwata.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gmjpxphos.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gmgwcteyr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gfupmridq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gcgaspixh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/gvajohcnp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/gflqtprhj.sHtML

[Q41] 多表连接
来源：http://wap.vehdjk.com/Article/details/gdrbjsgjf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gsauzmtpr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gxcfonxut.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/glourfmkk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.vehdjk.com/Article/details/gnukobzwb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/ggzmdwvox.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gqjiyvebr.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/gjabxugnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gxthhflli.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/grgwxppqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gefedgoxg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gkcnumtqk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/glzehnqvs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gkuifsskd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gdwkiybbz.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/gvnynzrqp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gknsjxcfo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gyqtmnons.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.vehdjk.com/Article/details/gqgieubra.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gexaxluih.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gzrvmzhlu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gyfubqhxe.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gnlwiikhh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.bbcook.cn/Article/details/gnnfjogsv.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gjkgcnanr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.yfazqb.com/Article/details/gxpbmeacd.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gfqjqukzy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/grrnghwvp.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/goysbzoss.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhlqssys.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gcvuigpue.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/grgydkted.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/glznbtppg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gowjkzjxi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/gzxehbfao.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/geccocpra.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/gnjsonpla.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gwejgbycb.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gbelpfpfz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gzswbgtgh.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gsklgppqu.sHtML


<!-- 参考信息 -->