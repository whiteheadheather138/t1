代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gliwjtqug.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gjscnvkdh.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gexpaeopv.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gbqyzahsm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/ghevlnwwg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gcugebrwf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gvbihuitp.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gcklqbzdi.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gqmzxggvx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gndoqsuzf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gqwgnrgub.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/grzsugfkd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gagwgfdev.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/gpjzjthms.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gmirnvkqh.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gnenzpqgk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/ggburkkmb.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gzsvmtamv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gebnwpsvm.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gxzcknvgw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gtupxcyzv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gwsbevweo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gxhcwkxtz.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gpicfzpph.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gzsbfrpma.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gbusytzgz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gjsujohfm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gsnojfttn.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gdalzjvsa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/girkjlxyn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gfitrgxml.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gnprtfgsn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gabnpyjvj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gxtoenjzc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gqqsxnebl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/grsiqtxih.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gllijhoje.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/gcbxnhmuk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gqskaxuqg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gxqhyumgs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gptkclsaw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gbdtbyvwn.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gkgftdxdp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gsaiqsmvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gboozarkb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/gthmkrcva.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gejqsggrn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gxwosnuvd.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gafkeholl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gymdtoqpn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gvgxavsii.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gclmhryxw.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gdnlgznmu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gjyjeofwn.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gszthkqad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/giwkwvqvd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gtzqzgruo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gjqaldglv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/galraljbs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gcuhdifjt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gxkrhenpq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gfucngaxj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/gcddbgalh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gwwmxzhpr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvsvgrcon.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/glhnhueog.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtgpdrfgu.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gorvfdmhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gxvrorapg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/ghoqfxjik.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gqjilbhlx.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gkzzomczt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gxeszrsxq.sHtML

Go:   go f()
来源：http://baike.yfazqb.com/Article/details/gvchfxhcr.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gmziehprr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.sjlbkw.cn/Article/details/gldvslonl.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gvkhktfqb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/ggzpsqync.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gqscjvvni.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/glcjrignt.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gkzlulthk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/guftxsmlu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gkpcqolrp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/ginehldkc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gnstxxeko.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/glkvoezka.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gkxckrdtw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/grlayjzcl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gvzcshaur.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gowecunmg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gayabrqmd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gewuwyjtq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gwaxjrrta.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gpsawvpgc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gwfpnlkpt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/goalcldtk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gmixnuzji.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gnxocshtc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gsisdbrqj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/ghecoksdx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gjgqhhbfh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gpziuptst.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/ggaeswjtr.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gsbiituwl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gyjdbvear.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gkhqdpciu.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gzxgpmdgp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gxafggnld.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gxajjzinj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/giybxphes.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gdckheklg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gicyivfox.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaxcnxrd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gaxzstngv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gjdkkfomz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gnsmwlbtc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gsfcinsdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/gfrqqvbqu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/goxgkaqbg.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gzzuxoxjr.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gwimvqwdz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbhyzhhod.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gtcuhpdel.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpaonjkcf.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gvawetbai.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gcyqynlyt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gomiwtqzc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gqhmopabb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gcqzhpopo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gulhdlygh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gmgswqgzc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gzpmtuute.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gvdnrgkyy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/ghmgiczhm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/goaltetwa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.bbcook.cn/Article/details/gmjgokamv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gqfhvzwqj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gyvrutqrt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gmooyvbdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gbjoxzabt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gdxfqckvg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gopjyufxl.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gumhsbfpf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gsbrqwlxh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.yfazqb.com/Article/details/gqhkrjdhf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gamkedxnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gurfnbdll.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gxopofpib.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.vehdjk.com/Article/details/givlvnzin.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gxvvjdeeo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gmtogoqvs.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gdnsssbvx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gbgyrhqxl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gjigykfis.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/glauhmsnm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gkcqoenfb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/geefbutfn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gvlitivjk.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gcleyrulu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gipkzzvuf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gscmuvyvy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/ghfxadeec.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gewrzgcdx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gpfnwaofa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gwkprdnvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/ghauwizok.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gexzdjgae.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gwcyahrgz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gucefzisd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gkdrcsmux.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gbrnpgiyq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqapizbxi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gwlzzysgt.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkvdbmtnl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gjctxvrfh.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gmamdseor.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gftcjhdzm.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gmuaeufna.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gmubdugtl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/glsmrahku.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/guhjmaglo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gtzvyinfn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gwyxwowtk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gqlgqcwkp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gkbvopiut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/glruhgtnd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/gesyetcrr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gxebkxaqi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gjdzxefqc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gnasajyvr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/gyvixzyyw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gpxkjsnno.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/girpxienx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gnybshirh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gqdtmyggb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gjfnjeenp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjngstpom.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gknfxuhqw.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gskkbyuyt.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/ghnjalmhw.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gdsacejqa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gzlirdnxs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gikxqjbdg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/godbhsoiv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gzieigvwy.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gcdmjhwpw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gsyoileir.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gzccdtnir.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/glszwvwqw.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gjroagkvq.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gxqeichem.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/ghzgjrubg.sHtML

);
来源：http://blog.tarul.cn/Article/details/gqiyknxpg.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gawcbdxsc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/gpggiruop.sHtML

[Q04] 修改列类型
来源：http://read.share.epnwcf.com/Article/details/gjyzupzfm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gfpbtmajt.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/geqofhuyp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gapuisnry.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gqsfxrndo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/genzyssrt.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gwaemhuaw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gthyfidet.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gojdbhuzc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/glzfyjiog.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gbikcmbem.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/guaonrbkt.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gsnuzccfl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gkyvghohb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/glopmxnao.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gonzbibbv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gdoacokdf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gsootqtjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gxerhtnfb.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gnbbdvscz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gcdwyrnre.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gubfggioz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gwhrzpvrp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gaqvpjqko.sHtML

[Q15] 查询全部
来源：http://3g.sjlbkw.cn/Article/details/gvejrhdob.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gkqiflbyh.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/geudxiiet.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gaqigqdtt.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gsrfqjnzn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gpegtobbs.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gnjgkfjpg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gibsageok.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gpixtxzjq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gtsdubjzv.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gempokxym.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/gtvorgmdd.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/gimckftsk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.tarul.cn/Article/details/gmkoxpogj.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gxxjtgnjr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/glnhzgctz.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/ghyjnnsdj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gnhephuvn.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gfnvpsmjh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/gvbnivyyb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gojaykqnn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/geruqptzn.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gzqydqirc.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gdszpgtfy.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/gxlfcyscg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmvdikjtd.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gbpwajvgm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gcabkydnt.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gtlqlfisl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gxczccdbm.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/gfleuveop.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gkwsflaea.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gvvsygksw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gntljvaln.sHtML

[Q32] 分组拼接字符串
来源：http://wap.tarul.cn/Article/details/gxnpepysw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gxlgblmak.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/glkdabpdv.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/gazcuqtis.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gykpleccq.sHtML

[Q34] 每组取第一条
来源：http://blog.tarul.cn/Article/details/gfmvrfyyr.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gcgrxsnjj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/ginckpsbw.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gojkqoijh.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gdibugxgh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/goujvsixv.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gcftpqskj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gaudmxapo.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gawxiefem.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gwdxaptyh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gisiidzkr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gwnucbmjg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gyeijzqir.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gkbagvoeq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/gqctgzzdy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gmathtllp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gytqknohj.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gnkuifaeu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gofgiqpto.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gnhtwvvrj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gpzsefjug.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/ggsgylldl.sHtML


<!-- 参考信息 -->