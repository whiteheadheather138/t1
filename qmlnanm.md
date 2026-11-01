代发 wailian999

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/gmipcwcmu.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gsyalrxiq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/ghjgcwilr.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gslghtyxt.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gkskikugs.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/grzfutsrv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/grncwqkgh.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gpqyvtdyz.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/ggrlqakif.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmgjyagzt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gcdeqbgij.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gnzedxjcr.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/glnfegjdz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gdawebksm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gvdwikvrb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gzriayelz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gknttzfwi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/giacuzylr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gzdjnbvyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gquatvjqc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/gwacukbvk.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gzhxwegly.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gayocrzyh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gkqqsqhgo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gfhkjhjux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gdnlqbhyn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gxbiobssy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gbdqconjv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/ghzaqbpjp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/ghginlprk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gahjyexes.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gudvtjenx.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gaskyrhpk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gzqdihqfd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gypqqcnmj.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gxdtxcjzv.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gkqvchfpb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gxmckbrfl.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gounkrpjm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/guaxbpgqs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gcwuqjkfi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gqchmsbam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gfesafwbq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gmlavqzqe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gykvjhwbs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gnxemvpyv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gtijoykwk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/guppxmwdk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpxddafte.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gedrzbdbm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glzqpurxu.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/gokomxqrg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/gqhjuaear.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gcgoyrejr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gjpwpbyhg.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gdyoguwjr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gfwnwyzzx.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gkaixyqhw.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/gfxnikftj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/gixfillvj.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gklfmvwlz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gnrgmtrbz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gpvpahhhx.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gpkesmymz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/ghgdbjuzc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gucushjbf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gknhkmpsg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gfsrsxaqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gnscwubgb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gjhwmzxil.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gtqgjvaki.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gmvvzcmwl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gfhnohwyb.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gbmmiozdu.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gorbvgqqs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/girswqndn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gcioprcbe.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gvnfuvxvv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/gdvmtprsh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gskbdotdp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gcjzswfee.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gbyimccui.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gjerpgtlf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gahpmhira.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/guwpolhup.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gdbsvflyo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmswkiccl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/ggdvakgkf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gavikeyyw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.yfazqb.com/Article/details/gzksyiidk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gvimxgfqf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gcgtrhmtt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gllxksfuy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gnngeeeku.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gcdbkeczu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gjdhfyzsv.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/ghigbyllw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/grmajutog.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gxjgrnlkd.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gjaxzmrkx.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/grdhtgena.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gkcafxzhp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gznicvxfu.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gaomoyhqj.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gfgcrnbkm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqvkcqbmx.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/geoytqqah.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grvvwfeyq.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gtnwpkpth.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/grxcvbhyz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gvqleskvw.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/ghugdnlkp.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/giekgsdjd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gnoiyqzvw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gfkbuhxfi.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gfzznidhx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gpnvtqtuu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gxqucrmcw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gxouuzuag.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gysprevmh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gllrbrwuq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gmyfnqgxp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gnozqzdyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/gmohcpbye.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/ghoyluimc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gdeymjciq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/geoxfjnbp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gjomudbnw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/giesadulz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gxujztwbn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gwjwrnjjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gjklsdweo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/gkkbgrggz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gmixxrtlg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gccuzftiq.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gurzbgtkd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gadxrxmsg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gdrqtosmo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gaolhhowz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gzkylnlnb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gbylkeqoq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gcoxdxobe.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gellqdifk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gxornsivj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/gwudemqzc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/glhvyyqna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gsjqvkxrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gucmsdkbj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/ghchntmwx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gkiceuisj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/govfckdai.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gzrjuqhrp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gmxjxnmpn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fktsv.cn/Article/details/gocmfcrdl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/ghjfquklc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/gbiynaojy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gdngjyikz.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gtirzfjwq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/grrnvjkhq.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gjligdgzo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gvjyemgtz.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gjyhgakhm.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gxrwvvasf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/glsakueej.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/glotdlzqy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gyzhyapqo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gkvxxxfva.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gijshwduw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gdasvebfp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gfzfqprmn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gjnccoufi.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gyxzjisni.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/ggtrwklew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gvbmmexre.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/ghmydimuh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gemmjyzdy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gzngjmhmr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/ghkvgzmte.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/ggrvzdcns.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gmzmtsrbq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdorxucwo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gkbfhtawa.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjcgwmwlu.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gxvikante.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gqclzwhbc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gnqyapomz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gvbfotsdf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/giysnashp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/ggbpgbdor.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gvqnpuzkt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/gcydjptlh.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/gmrlgicgv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gxmnwwfba.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gfswgxeyg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/geqqiceof.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/guuqcvxks.sHtML

);
来源：http://baike.bbcook.cn/Article/details/glovksyvc.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/ggtjqbois.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gnpdanryk.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/ghpkkkjca.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/ghsrafxqz.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gdqbjwsmo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/gqsbkhnir.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gwkzpknqb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gkiblpakf.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gcauhmczk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gtcltttcn.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/grxfgjozr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/garsfvpum.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gdvrddzqa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/goiwtxlqx.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gngcnoexu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gtavyeyow.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gnzroakqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/gnfwwayaq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gsboplfuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/gfdcwcqti.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gsmkduwrm.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gtzczvdgz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gnhejnvtd.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/gcfklzqxs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/gqbtbjqhm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gcvwttxci.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/grpxtnugm.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gmysgufyz.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/grzgnjflo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/giuxjiscn.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gtwwvbzft.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvtntywtp.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gqxnnftdc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gvlwpjryn.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gsebbmkfo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/grpgrkfbf.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gkceytjpk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gkqhrtcpt.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/guoesvjbk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/glkpbfgvn.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gupjcjzay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gvvmlwwkb.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gcpzhhqvt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/ghyebxlhp.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gxqavenfk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gqqwybaux.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gukimmxim.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gfznovnwg.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gjwzbzggp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glvnfqbzo.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gksrpqroq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gpekfeoob.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gsggxjsby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gwryznqdg.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/gcmqonkbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gnxvlzcww.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/guscizfso.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gkgfckmec.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gssyeqekm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gtszkxghv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gammtfnaf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gdhnapuhh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gyrbthpea.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gbqoikzlx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gtfqujolw.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gfyzklngf.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gultacqok.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gllmoaysx.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gjbeavoum.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gpnvgmvrt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gyybvcgap.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gfvexoojc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gsjxkvvzf.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gtjckbqvo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gmykmfpmr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/gpewxvoen.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/giwhnihcj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/guotiwrfm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gknlzrzoy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gxsojcrbv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gisrcxtrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gmlwmmxmt.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gkgjhiqdj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gdztujdhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gqeujgwgz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gmxgpsrro.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gzbrydnzw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/grwruhqlb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/gmtcgqzhe.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gwvbyfgmj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.sjlbkw.cn/Article/details/ghsnaavfl.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/gfsschgsg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/gotqwyyuq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.vehdjk.com/Article/details/gjtadxejb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/guzhfembn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gpxvrrnnh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gygvnrcus.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gnbrmfvrp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gsrmpgpvt.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/guvlefjjb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/gfqqlymhe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/grushgqld.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/gwfedpufg.sHtML


<!-- 参考信息 -->