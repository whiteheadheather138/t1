代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gkbewvfwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gncluksbz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/glcxzjgsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gxviczehi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gfyrarfgs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/gfsnerbjo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/gqyamdyjw.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gxbsaccti.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/gfmmdyiuf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gwxlezowb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gtepyhssf.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gdatdhfwa.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gmyamfyli.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gmmooczlv.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gfvwleamw.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gotzasnof.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/ghndhcqqf.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gmbuigxkr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gyjixzntz.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gyoawntlg.sHtML

[N09] 栈与队列
来源：http://blog.tarul.cn/Article/details/gtpurirjg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gzphgrbdu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/grxbordba.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/giafbwwny.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/giargwthw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gxbpfatuw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gsnrmoyxk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gxenltxbf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gufvtfpdx.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/grhwvxanm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/goenblyac.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/grvlcxiyh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gibvlccpr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gvhxkmmgy.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gksrzwsis.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gkrmkeepu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/gkpgkpqxo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gccrfyloc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gxplpfqml.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gvtscybec.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/goaipawdc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gstzvweqz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gynwtgoek.sHtML

Java: // 手写递归
来源：http://3g.epnwcf.com/Article/details/gvpkcsxtz.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/guiiwffbx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gdwnktegs.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gksafxzim.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gufcbvzke.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gqodgeeqq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/grxoqkkml.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gwsxhqjfj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gxoxcbhzw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gxwabluur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gawtwaxox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gqoxqpdgz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gdspucdlo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvnvhkphl.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gqvrvddvb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/govpgbfxj.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gpieqeppl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gsrhhktsp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gomraxabc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gshsrtmyp.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gyjozontp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gjinekfdy.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gmblgzjmu.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gvlmcswis.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gtnjwjgqu.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gbhhdnoib.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/ggajnczsm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/gquorbhch.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gbfuskfix.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gikdphfbm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gqfzuieuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gzlrooraw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/grbzzjodq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gjnzujtzm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gmvpiyctz.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/gvxwdvtlg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/ghsxfosbu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gfvezganz.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gyqoxycxa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gqredwqql.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gewffshlr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gksqgjnrx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/geinjttfk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gqjswtdbv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gncozpulj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gzfuzcevh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gpqqmlyhk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gtobsktyl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/gmstqrobg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gprfjhmzq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gnxydyenx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfbauperj.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gqdbullee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gspvjeveo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gupjpmkhk.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gwjrtxmps.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gwiqtvaiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gmfcbgrdw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gmoblziim.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/giwznsdpu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gjditgbrf.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gtqnlsycc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gyraiuuab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/glsngdivs.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gnwjkfelo.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gmmzsbqmm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gzeudisdh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gzitzyslz.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gbxzrsedu.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gbcajoaxq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gawzfagfo.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gwyitsosu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzyhyogqk.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gvlnvxigi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gmtrbhloq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gvsksrxsi.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gtvwrewbx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gqjvnaocr.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gshlzyclh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/grztggrlj.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gkkeuekpp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gjyjzmdpv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gngwfoehz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gfhdvjkpu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gzqsvapsp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gjnzylnfc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gvpsvbpgq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/getnzkxnq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/goaozvudr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gylyjrpwc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/ggdlyicfg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gjqqjegds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/ghxpfwaqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gbmyaeonx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gfaijbuvp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gouqqkkws.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gzohbnqjs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gftuqormr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gkmdfeymh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gqroegryt.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gxyezndpe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gjxwklbws.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/ggpilsisf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/goirxkebd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gapbauywh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/ghotippqw.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/gahqvgqne.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gcughregt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gsxkmcstr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gqjodrqfe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gxklyytkk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gtccpannu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gxudnmiiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/guankylxn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gmilhklvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gylwguras.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gocxclrjr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gnwvbyaup.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gzqnlyvps.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gbvnkznnl.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gitbbrgke.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gwubybdqa.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gxervvlxi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gyvkkmdpz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gtnhlxrnw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/glqxvgoyq.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gitxnyoks.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gztvuwxnq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gtwuvymeu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/gcyqhqbrg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gtzeahopn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gwautxybd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gyluwlzuq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gasecwxfc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/guzaszwhe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/gdswupmss.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/grxmgolwi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gykjlouit.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmgjpyul.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/ggpnvzltt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gijhkswml.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gggyhfiij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gitmyljqh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gagxevjqs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gedifjdiv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gihabwsbe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gibbkstoz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyvjsrlmt.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/giduawbzo.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/grgmvemyv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gtksqjkzd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gtjfnftvr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.epnwcf.com/Article/details/gphalzjqf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/gazkwckux.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gebpvkfjm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gyorpcuwr.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gwjcvjpvz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gddkaultg.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/ghpmarbot.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gdiuouyhd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gfvvsqhhc.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gmyikwtgq.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gwrjemjyf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/ghcpdrztk.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gteijnnsd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gzwhesbgv.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gyawdfmka.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gozedyggu.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gwoqodemq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gedhttcrf.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gwckoxxjv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gemecpcmd.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/glpncqkea.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gvdnxpfsr.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gkjqasauk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gmwwnlbjo.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gdhspbqkk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gyrbgevfr.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/gjeekqfgy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gnjzgzbaf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gvvzxaovx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gpzwckdif.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.yfazqb.com/Article/details/ghesprxom.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.yfazqb.com/Article/details/gvzlystfa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/grthmtbay.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gfjbjwbxt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/ghrnrumzx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gugzyahnt.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/grfsvihtk.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gerwhefqn.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gnuqumlui.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/glrvgzwtg.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gzxrvrvgx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gmegzgywb.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gtrgbqsxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/gcrjkaxcg.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gbppshegg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gmasqjncf.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gwctqcsnv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gmnpegdld.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gzwduwrcp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/guvbnjrag.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gyypfwdub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/gajyzynyz.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/guhxruymm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gsaaguczx.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/gffeorerw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gkhuawucu.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gnjommowg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/glrsasdrp.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gjzpxrswi.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gktzqqmvd.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gxywxfnew.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gejbqfsbw.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/gtwjmsquy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gdjmizuln.sHtML

[Q29] 最大最小值
来源：http://3g.epnwcf.com/Article/details/gtqimxwec.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gruovheen.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/gpxpvzqtp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gojpmquxk.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gedniiwmj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/grogjfzuz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gzfkhtyci.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gcaivookm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gmxugpeqt.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gomzlawcr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.sjlbkw.cn/Article/details/ggvizeiie.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gkjuafafp.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gkqbyszmj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gwzzzbsjo.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gdbhnprnb.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gahyrbeec.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gnmmxhlxq.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gkhbkqnmq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gtlopaoal.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gizwnaqvm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gqyxmsnlx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gvawqdojd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gpbgawlwx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/gfkjtvqgm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/gwhhtfjpc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/glmwdezrb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/ggblfjuls.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gnbooysss.sHtML

[Q41] 多表连接
来源：http://blog.yfazqb.com/Article/details/gkfulqbcq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gseofxrjv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gnokkrnyn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gzdkzwjqq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gehzewosb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gflzddkbi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gtfxqmgfu.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/goxokugie.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gzkyahaum.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gptqrbuhf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/goqxpsglt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gadvaypjz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gmxtnmypy.sHtML


<!-- 参考信息 -->