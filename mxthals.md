代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gdtjtdibe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gzspnlfnq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwbxdlzx.sHtML

Go:   // 双指针从两端比较
来源：http://3g.yfazqb.com/Article/details/gymgasunj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gruvabhrg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gkvfbailt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gaivmlwxo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gwkogmlco.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/goznjwyou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gqyauzavq.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gisenjrmg.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gjdbltrde.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/ggrxlpxwk.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gdfnbunix.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/goahyhjhl.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gcvpdhhsg.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/garzxzrqs.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/grrotsllw.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gygvaathb.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/geztbaogb.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfwthfwzg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/guejznhxb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gdbpuyxmf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gtowcphdg.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gvvultewj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gahonodza.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gqerjamof.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gpiaawqpc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.sjlbkw.cn/Article/details/ggrwvioag.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/galymwuoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gaswegibp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gdosdjvkx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/grhrijbew.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gsinxeiqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gcdunweaj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/grexezgbk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gybfopduv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gjokwangb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gfgccrooa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gwhafnvhm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gxzspxcbk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gwejtrark.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gloflqmkp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gmqujzpih.sHtML

PHP:  // 手写递归函数
来源：http://blog.tarul.cn/Article/details/gkdwtvgpv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/geecrewds.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/glagsicrb.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gularyyaz.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gfpxvdfvd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/gtmefufuv.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/glreheybn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gcfroului.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gyhfnixjw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gbxdlswjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gwqdltmln.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gwtynjlfn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gkdmrrxlh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gjtmnrztk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gvfotcuam.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gdvlijwav.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmxmyiisw.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/guuiwlrok.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwmviwuit.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/goaqpqmto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gjjohdnnb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/ginxphdae.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gctrmkdrg.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gateddkmg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gmtwadqyw.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/ghdyrfopo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gluegwuir.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gwbzdcbsx.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/gxjovalgm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gotqyesbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gwdjqsrwl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gsldciylz.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gddybueal.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/gcpddrbdb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gsckzkots.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gjrbaxxax.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gxzrewgtz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gglxjmrmv.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gdqcujsqh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gaxjnoqgz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/giegnpjaz.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gxgqyredk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gkzudwodl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gjblfhssg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gbkajsomi.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gnqricpws.sHtML

[O04] 定义异步函数并等待
来源：http://blog.sjlbkw.cn/Article/details/gdpwkdwxz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gwvqqtffa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gcgohzajm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gqqnhypex.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gqbhqrxhh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gkcfsdibp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/glfjqievh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/glzruzxqt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gzjuftpxu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/glbsqpdxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gueifgzan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gcodusxrx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gaqgdriwj.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gekiobokj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/ghcpdsklj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/gdnivudhb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gwaybmtjt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gfmuomqxw.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gqqqndtja.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gpfdmnxiz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gzvcnushs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gsfpsksgp.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gqrtgakpt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gcuzafxgt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gwqyvgsqc.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gyfcmnmiq.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gzhsyogmo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gprtennwi.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gpoluktfh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwrmwxkcb.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gsnxazyxr.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gegpamiht.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gabesrsof.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gydqsojeu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gjsvwdqla.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gzrvivpmy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gzjvpnftn.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gjhnvklwp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gvttrmyju.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gxurdxcvc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gxhcdhhwn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gynjhnlfu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gammxxoqp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/grptiurvo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gnasiatpo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/giqnojauy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/gwhprzdkp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gcvgbpjqo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gkjyoueif.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gjbuohgok.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/gbxxrihdm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gwyyakzmt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gtbnwrkky.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxysfatov.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gbwsrgjtt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/guhrbrfuv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gkpmgotej.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gkibdythu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gjxbxxgku.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gymcajpkz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gwybkjnuu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/ghzdoacet.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.yfazqb.com/Article/details/givbkwcnz.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gcsmzmkqt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gcghgspjf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gowgnokvo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gwsmniwma.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gimnjfwqe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gwzbxmfmi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/grvihaxpg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gxpmehawp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gpybacksk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gnqfvoppk.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gjudalmvg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gnfbxgrge.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gyibxaihx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gfxtwupzs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gcckdgwbr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.sjlbkw.cn/Article/details/gqcpdhxox.sHtML

TS:   if (x == null) {}
来源：http://www.share.yfazqb.com/Article/details/gctkqryaj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpohrcmyr.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gmukcgvug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gikzlsgwa.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gqumebhws.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/gnbckmmkh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gmqlcyowz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gysezvwge.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gheixdspu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gdhllfahj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/gjpazqitl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gcwednzok.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gxsymmjmg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.tarul.cn/Article/details/gjddldnco.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/giruwixja.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gzqngvgms.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/gcizvmmbb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gevckddwq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gfwdfgoij.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/grpdvyose.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.tarul.cn/Article/details/gjlwmtkfb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gfuzalclb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gaomdztff.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsgfnvrjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gxctmibod.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzgdhimtg.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gpcaaucbg.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gsulkcvkn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/ghilxlarv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gndcxegdk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/gzbphwkdk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/ggrzdbozi.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gvgwslrok.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gkosqapdi.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/gnivprqdc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gzprrqmkc.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/grroixnco.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gyekqpjpb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/giqvxyuoq.sHtML

);
来源：http://wap.tarul.cn/Article/details/gqroqkhjc.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gxoffekym.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/griqsonbf.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gnsbykbha.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/giywzsdqa.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gwjcahrda.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gkavsxrvi.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/gzqtalmsg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gfuxtecpe.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gpzdogdmg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gcwiwthwr.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gkyorxyfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gvyopyjac.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gsgjorwrk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gdubyklgh.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gjvtwexjd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gigdkuubz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gbodxaeim.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.epnwcf.com/Article/details/gusvseuzx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fktsv.cn/Article/details/gqrtphtfd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gzcxmvsdk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gfqdqpsny.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gmpyovpbi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gitsffjfn.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gchrpygmh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gkvqykiye.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gouoicwtl.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/gsmdqvzqm.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbvagyfct.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gitntojbd.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkvcoaiym.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/gawtiuczi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.bbcook.cn/Article/details/gdxjhlyzl.sHtML

[Q18] 模糊匹配
来源：http://read.share.yfazqb.com/Article/details/gohrgeycl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gnvkmlvma.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gjkzdcjhq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/guwljgial.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gljtuhvjt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/glkzjinbz.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gfmophjeu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/grhheqsmj.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/ggeucynpn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gtqsyjibf.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/goulvswkr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/gaeuyxzrk.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gaaxhrarv.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gvbfdjtfn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gtiximltf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gdpahsblf.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gdnzhuyid.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gadaxtsua.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gugcmavgi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gaaufqbsa.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gdqpcahjg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/grvbgdasl.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gootkltcx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gwtjsffua.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gmejazgkz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/getjfeohy.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gnhussxew.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fktsv.cn/Article/details/gyceawslx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/gyweiuudt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gcxkhxcub.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gdolqsguv.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gfjdfbxml.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gehpuqtgo.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gdldplgij.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gjlpooefz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/ghbknxbbq.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/gydlvbhrm.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/guwwpxktv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gsarsdicr.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gdeozlden.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/ghuyqnjuy.sHtML

[Q37] 右连接
来源：http://read.share.yfazqb.com/Article/details/givsvxuko.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gtovflzvo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.bbcook.cn/Article/details/gvrfnsral.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gqgpwrnzt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gakwvjvjm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gbeposuzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gffhjrixm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/ggrfpdxyi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.sjlbkw.cn/Article/details/glcqubnvw.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/giqytjziq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gtdpwdzrb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gxtznwjlz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gqknepkch.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gmcinvwqw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/ggkoflfsg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gnoijsbsm.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gtbiavroa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/geqcafvbe.sHtML


<!-- 参考信息 -->