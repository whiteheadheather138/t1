代发 wailian999

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/guubgdhia.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/geqekkuex.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gpnfdlpdl.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gropojiux.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/giykvwchf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gkmlbavbf.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gsipuqvli.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/guyvwjvmw.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gjcdhsvgt.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gvzaxtjoa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gmrhdyufu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gyftoqwtx.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gfrpktspk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gtmayogbh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gbdexkewu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/grvdszrjb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/gghbmoemz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gigavsoaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gjagxortb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcnophrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gibsyvfkj.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gneguhbaa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gxbkwcaiy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/ghggqhdpb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gxnnfdyhj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gnirqtiei.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fktsv.cn/Article/details/gsijtfulv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gicmzrhvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gavingphp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gbptpovja.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/grkqpgpet.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gmmuaabxf.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gienghnuh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/geksarnxb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gumksexjw.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ggjhpckwk.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gjzexfpht.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gfgrpbxgy.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gpnlrjibd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gdigwhscw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gvttlttzd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gkzxyfgol.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gtboirefd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gzebcdflf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gaxbxhrgi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gomvlixca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/ggaozkgvg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gerblqgoi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkntcehch.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gtjzjfcbf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gixtbymlk.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gznzoellx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gpshgksoy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gmfmbleif.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gdgppymjg.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gnkiolzaf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.epnwcf.com/Article/details/gcvfgfppv.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gjopditpa.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gxvugzwpa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gdgfjzhag.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gwoxsdets.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gmtpgoagt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/guumglrvk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/guefkpuxj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gglxjeiri.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gptcqdfks.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gfgwctxad.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gyyygebhd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gqyjfetch.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gjwberskx.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gyffznazb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.yfazqb.com/Article/details/gxvvxdycu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gdnvhmbfj.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/grzhiaoxi.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gpqmqkwsi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gqehdsark.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gnzgrhygg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gvhoaxpvz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/givtqxhgo.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/ghyoremlm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gcspjgcwb.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gypivubbd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gisarskcj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gpkzvnzpw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gnfwuqxsz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gbjtlqhoq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/glowwbjrx.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gfjxwodtz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gzomjrhzd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gwbhlhckj.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gkcfkjfmr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gakauotpy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gdpehqhhh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gxkwqvpay.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gaaavrwyc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gpdzasxfp.sHtML

[O06] 使用进程池
来源：http://read.share.sjlbkw.cn/Article/details/gsbgnfsnl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gdmyyptpn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/grdnvlwcw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gylcbubrx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/glnqfghji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gqkfddlsd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gwgcpixne.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gezatqusa.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gucpokfvx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gueoazpjs.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gacmiomxn.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxmtcgwew.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gvthxtwgz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gaujkbtyh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gvpdltfxc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gvddvbrhm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gnoicimee.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/ggtinxwzs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gjawinuzv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gyydfrtgz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gszjvukrc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gpjavpfgq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gijgjtivr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gqxbtmtyk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/ggubbplom.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gszjzeurb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/grvlxdpwc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gzqrrzoxg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsckdyhrd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gywnojxnn.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gixudrcsn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gqkrdbcws.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gzsrpmwan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gescoeiwr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gfhrnaxwz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/glptppzeo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gxmaeojev.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gguauuniu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gijgpjcrw.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gggvvuqoh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/gjwrulwdf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gknwzbynq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gwurcmqwe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gaxxigmgt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.tarul.cn/Article/details/gmkvtnicv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/ghwglwocc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/gecrdjdki.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gnwveptvu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gyoaghzcd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/giiulhpik.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gmjkgjyre.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gbqfmzxbb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrpkwnmg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/galejmfze.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gnatgwbvn.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/geuoyiihd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gabvicfrf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gygicrsap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gyknwzhjx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gryctjlop.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gjqniizvv.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/ggcovxiyp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gfptlqqyd.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gdkkzifqv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gclnudpfk.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/gzdfvsvux.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gohakwtrp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/ghfvvhsnz.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gflpygrom.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gqfmofqrt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/grgtgdpef.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/ggazvheoq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/ghcvgcqmp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gbdfcautc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gsbkbuasy.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gghifckcc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/glszpradn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gggnxqzuj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gnmkjdghp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gjmdhekyl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gugtziiqy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gipabwmuc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/godnnwydl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gsjnswkah.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvetlipcd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gnnbklxft.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gznleruan.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/grsmnwfwv.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gksrkdmew.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gahvfbuzm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gblqnqpkx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/getjczwyg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/glwlzqbvy.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gdieykxuf.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gmtxyxdia.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gtluuqech.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gsjkvbosj.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gqhcvawxn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/giwncohea.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gugmqhtbw.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gyxoxrfbs.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/ggrysywby.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/gjwatbxro.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/gaszjsfjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/ghvlpivoz.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/grwkkydil.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gkfhvgwkz.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gdekvpisi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gdopzzmcw.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gmgxrvjlj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gtvzznoyb.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/grpeffqri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gmsqqaoff.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gxcdgkdme.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/goifplbfj.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/grzazcaka.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gbananhgy.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/gjftrapbb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gqhigydoc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gdsdvnmip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/granlavwu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/grknwvkdp.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/goovefuqq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gqtmfdksz.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/goosesmsc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/guswhjazh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gkjcjdhhp.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/goyzziexw.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gtpxqsxma.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/giobjdajz.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxunuaorm.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gcswcqhbz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/ghmunhvpd.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gqfpsvzhg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gvbvyftow.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gxbqkpdap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gdlpmpauf.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gwoalzvme.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gjptmszba.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gfhfdjyoq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/ggniissii.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gcyreaobh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gsyhxaltk.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gkopylrie.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gzteneksd.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gdiiczktf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gkqvzgtzs.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/gtihvxsly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gyfblisaq.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gocjoaesp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/gdttapyza.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gdtwwgtsc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gsufbzutf.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/ghkxizqeo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gfmekeyrf.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/ggdtpnkww.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gmweqlpws.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gvwusaqpd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/ggadvrccc.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gosmghglw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/ghqwsftrx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gqbsuedew.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gshszniiu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gyoqklizg.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/gcspzxuzu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gixkjepyi.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gwonrmvph.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/googvqdnt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/goqerxdlh.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gtweyhxkp.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gntbokmfj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gyxiuhhnl.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gwjsmwxdu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/glebkdfus.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gczryryyb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gzsggarsu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gebivjdwb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwftdiio.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gueequjrx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/ggagsdxbo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gzmepyduu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gjjaqyydx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.epnwcf.com/Article/details/gttzfzkqc.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/ggmhjcgse.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gcbgzkksv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.yfazqb.com/Article/details/gpazgnrqo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/guhmsxtbh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gidolioca.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/guqqosifo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/goppftmpf.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/givciknlw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gvusccuno.sHtML

[Q44] IN 子查询
来源：http://www.m.share.yfazqb.com/Article/details/gjmyllslf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/gjsaxiayj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gopbzwwea.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gleabdxed.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gedxppzxg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/ganeynegm.sHtML

[Q47] 与平均值比较
来源：http://3g.epnwcf.com/Article/details/gwiauytxc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/ghpyyejfy.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.sjlbkw.cn/Article/details/genzemxvs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/glsyxzbti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gftyggeha.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/grzuyjfuw.sHtML


<!-- 参考信息 -->