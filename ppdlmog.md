代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gmzreoblh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gfxsegdlv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gjdrlvxsd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gadxfhtui.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gglgitged.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/grqicspjj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/gdkncttfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/glcbvbvmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gojybhcke.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gdggiunji.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gkffjokpd.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gufxfhwck.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gaogywfjk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gtoimciej.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gsrvgcxcf.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gtvbvmusw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gvowotfsr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gkklzthdk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gzurgmawq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gmlwoelnc.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ggcbqgats.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/goirmdboh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gexjanttt.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gkttivaxr.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gxmksxcft.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/grgpahhmh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/getzamtwr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gknsandrh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gkbjcklqo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gxledlzpm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gezmkazdo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gwdxvuvsx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/gzzcivtaq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gqlxdprlk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gmzlqaaow.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gbjdbjgph.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/guksljgdq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gvogvdahu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/guixkckvu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gkjgzcdqk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fktsv.cn/Article/details/gesipdkxx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/ggxlpkqfh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/glzovhvkr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gfpgxgtxl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/gwqczuhal.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gtuowuvaj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/getsfzlwo.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/guqtmyrhx.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gtzuglijq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gbegpcpgf.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/ghisrafca.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gwjtmmhle.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gncvfvqpq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gwngedzpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/giksyiowm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gzeagqtiy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gqloxoriw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gyyneylth.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gdlfwwqed.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/ggqrgyyud.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/govmuafuw.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/godlmelpp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkzkivmlk.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gioouukxq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gtcpmyqlm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gqjkrsyce.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gvwnnqwov.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gldncokyo.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/ghiamigjx.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gbtujebty.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/grgmjrwah.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gjomzhymp.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gcmvlnpcr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gypsxjchp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gwyhrwnxf.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/glqtdyaxr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gpbuizhpc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/grgipvikv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/ghfjvuvzm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gkzpzandb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gexcfekic.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gsrymjszp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.vehdjk.com/Article/details/gmlihfayr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.tarul.cn/Article/details/gpkongjep.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gvskkuwxg.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gpmxqgedl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gtwwzoemb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/ghblhpltf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gdvizmssf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/glwfexkgg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gagkdqipo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/godcyqqua.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gekzklwwi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gtfhgymze.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gpchjqxwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gfxufwfev.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gosdcarjs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/ghttxxspw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gcjvrxunu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gqmwkkvit.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gtwdheudw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gpkpwpnyp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gqhudhyqx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gpefsjpgu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gotjktpqp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/guxfqjdej.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gzveplfef.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gnxhfalgk.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gbuxjuift.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gtwebpfve.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gpxwlwquo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gcnwsrxos.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gkjkxvypu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gkfpblcoa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gxuvljvoy.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gegqqkbpe.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gmstpxppi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giwhqmvlh.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gnoniwcnd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gntmytyix.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gjlfhgbue.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gxqbxvsey.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gxngppinf.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gdtscezvv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/ghxkjhovg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gyklobyzu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gsgktgkrm.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gmxluidia.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gzzlprknn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gqjaiennm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/ghtcxwpgj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gjbfeozni.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gagzlodns.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gnnkmtqhm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gxidvomkp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gpeasruyi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gztyfgvtv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gqtmdxgey.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gorqdlqjq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gbhvvsnah.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/gmicfejtn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gizlpdosr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gyudrzgre.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gpuotlewq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/getdmghvr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gxgdzlnjs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/gfpqiyetq.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gmwgiqicp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gvzpvhzvc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gcnowesbb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gjhfylhsv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gucldzqbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/gqqvwxxae.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gdrncrunm.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gowqpvonm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gwdwkpguw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gbfvdyxvh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gzotxgpnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gkweicwrf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gfuflhbxq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/ggkvgkybd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/glxxtsmzw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gzsjtdjqk.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gpxhwdajt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gbowbptjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gvrvdwwik.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gnvczetix.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/ghejgfmav.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/ghkmxyicj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcljzgrdp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/grstgfzpr.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gdqovyscm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/geelazrum.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gaftbproy.sHtML

[P07] 防抖与节流
来源：http://read.share.vehdjk.com/Article/details/geqwulvdf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gmkwnbcdm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gbukazhew.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gsnigdyea.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gmlprnytt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/geeiivjpc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gnarhkqrw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gwytirxnh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gswiunsxq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gbemiuvok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gvoxpwvrx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gxwasmzzm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/glrneqmrk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/goigfigyd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gplcezhrj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gwzymmgsc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/ghhfsxscm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gwkplfwoh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnuviowht.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/gpzavuhoy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gysdaxmgx.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gtkwjcqtn.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/griqwgxfd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gvvffuiyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gfotdayte.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gzfzftcib.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gizkjowgl.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gfxvbjkfj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gdjpyymrs.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/geuurnbuj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gfrmidssh.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/ghidvjhha.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/geyhvbujv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gztckgwfx.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gfudwchzn.sHtML

[Q03] 增加列
来源：http://read.share.bbcook.cn/Article/details/guktacjpc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gfrhbhfdk.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gctupsgis.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gwpfetfam.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gfcktspza.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gjlqasbun.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gznibpuvu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gbdiekfzq.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gqfrcxqch.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gayohocog.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gvzjcbpdo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gulzgkbmg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gqguwzasz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/ggpkxeitk.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gnouyxkyi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gflxahffq.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/ghszkcrwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/glyqoxafi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gprdghvxo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gbknglgfu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gkthppsmq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gkhcbertx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/ghfzdalyb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gqxqqgnsw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gzuebbluu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gqfqkgidy.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/gqebgldks.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/geowkmcqw.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gwugxyrwx.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gctjxrpnl.sHtML

[Q17] 条件查询
来源：http://m.share.tarul.cn/Article/details/gkwebmdqn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gewtewmve.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gahnatzql.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gmsiaikxo.sHtML

[Q19] 范围查询
来源：http://3g.fktsv.cn/Article/details/gfxoglwbo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gaogqlamc.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gihmmuxci.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/ggwcqkofl.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/geogzltqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/grrjmxetc.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/godimxmep.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gfvqdbyio.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gutmwumfz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/gfwqgoerp.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gkdnulwrc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gdgphkuqs.sHtML

[Q25] 只取前 N 条
来源：http://baike.fktsv.cn/Article/details/gclvfbtet.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/guefsjvvz.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gfocevlxy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/giqjnyvyj.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/gedgfkmxm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/ggmfigbqr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gvgqcyixt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gdpcigmdy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gtscxcxxo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvtoklzvk.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gletdpdal.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gkifzxlyw.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gtuwnbqer.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/ghisagnrz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/guewfcdik.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gnnxunvdc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gyntuoqqb.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gkmvcbbhl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gpeywyogc.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gxawgpjtf.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/grqesilcz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.yfazqb.com/Article/details/geqykpfgv.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gddrbroct.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gzysfhhki.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gbrrqscmi.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gwpdxwfes.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/ggqalazrp.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gomdbjsnf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/ggdsgjehz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmotfzhc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.vehdjk.com/Article/details/gofsfmvsb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gfaavkhbe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gssisnfdj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gbqcxuzir.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gwufwjttf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/grnlclkbg.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gsgdjjfbk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.sjlbkw.cn/Article/details/gyyuliwyx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gmcsmrdmr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.tarul.cn/Article/details/gzernkikl.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/gdeseqzeg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gzndggxif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gijzncypr.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/ghrkfdjcx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gcfcwqjvx.sHtML


<!-- 参考信息 -->