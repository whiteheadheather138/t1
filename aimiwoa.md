代发 wailian999

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/grvwneiii.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/ghzecfiwc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gfjxjfrws.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gbpthaqlo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gkgorwkhw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gzmjadyam.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gaouxxjhw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gclshvxuv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/glzlcvvmt.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gvbsnpqjm.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gfdsjvclt.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gfadanytw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gzjbnuehc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gvnbpgiso.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gbhmeuehk.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gepsqrtsa.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gpcoeckeq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gbrqcyczl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gtpckehfd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gncnabovw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gwmbvxvgj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gjpwbtvif.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gxgmvgsdk.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gobglomze.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gedsgrqxf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gwsayszwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gphrjlmwd.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gibqygvqh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gteefcrru.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gtptgnndb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gmdtyidym.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gbxdeuyci.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gagadtrrm.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gojdhxytc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gdgrcldto.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gisefsspu.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gzydmlumq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/gjsntfocl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gnsdzsodn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gyabemkqs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gvcmwqpqe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gitshkaho.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/ghcbbjtiz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gnhstogzs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/giurxdczg.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gzdylhgcq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/geibmmjyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/ggmlummxq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gsckmkwdh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/getgybjnz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gvnnjknhl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gnqtzgdhw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gjzbhlbfs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gesrqqtnw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/glrwgradw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gipkaopzc.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gbvdqfdpy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gvgqezihw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gxurgityb.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gzqsdbzbi.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/grttaabkb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gntkxmexc.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gounjtsmm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gjlonrerz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gjqyyctcq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/geujbdywb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gctovsfva.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gmalyztkq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gtealgwzz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gthhbkicf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gswsfcjna.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gwvphwkpq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggungnuax.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gkzyphqmc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gewbrdyfy.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gzojgjbsi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/ggnrjkyml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gifwwzrbw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/ggxktnfpl.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/geiedbihj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gaulowzwi.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gwsyhrnto.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gowvctpkt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/grbmvkrti.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gflycjwbs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gpwkipeeu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gejqzeuyk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gjutozaiz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gvuwliwgu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gzvypsghl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gzkssokjf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/goozaamkd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/grbxoedjg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gvvopvjwk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gsmuoffkb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gzfylfcof.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gpfmfeslk.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gzdxmmxzu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gckwtuaug.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gorglkjuz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gswzntsfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/ggespfomf.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gpbwjdarq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gxnvarprn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/gnycmshhn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gmkosmqcn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gzrsdtgya.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/glbbejkir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gsuvigafi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/ggrsougyv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/guvozgbls.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/giiygmwfq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gyjkteoga.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gegirfxph.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gddwwafaj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gwytkfcuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gxkbqjhnj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/godyjaham.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gpkqohnfp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gyshtxgvw.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gnqfsrnpt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/ghkjuslxw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gtaxbtrmm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/ggdittnfs.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gdeejollk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gqfcffjnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/ghvnlposz.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gcgwsmubl.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gmtfhoops.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfmopizzk.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/gizhhzlwi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grruuykgl.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/ghwdpnqyf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gnqmqryzy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gjwadpxtq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gdzqqmvsk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gfxtlgctp.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gprwugfrz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gugyuktre.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gujbkfcqv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gsthkktmu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gwilfsaks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gitrtojbb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gumsoiefu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gjkyfjpbd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gxtpfyvoa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gcnlnqaxo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gbhhlfupa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gmxvrynse.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gwwrvqovv.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gzrfchqxm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gqroxhbwv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/ghroeaywf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gdfgzytxa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gnnlwjfzo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/gijyngudr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gznlgbqfl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gdmmqiatd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gzpjoxdgj.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/ggzqppscp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/gahhlwbvn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gauascjzt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gknwtwqsa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gxtklospu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gywzyjhbr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gtsgqcjaa.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gurjovris.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gempxypvm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/ghyxlgttg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/goqjfpwfa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gxsxwefny.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/ghpicpopl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gylrxtovy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/glcfdoghm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gnkvvvjgi.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gwknnaolj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gtitlhqxu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gdtnjnvzx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gvyscflcq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gpfowavej.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gcxwybtsn.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/gogiiapbx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gpwtmushx.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gtejrlrel.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gpwszrjtz.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gheragbtd.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gexfkhcqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gmoqcvbdg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gfjozyvrh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gurftpgwm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/guywipkhl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/guvmxtklk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gahmacorg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gbkpthtkg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gqwuluttt.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gdiczpoge.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gstrnmudi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gdalvuwco.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/gvykolwge.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gprayxaqf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/grqmhtudz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/guhdshfjh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gljkvumfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gzvijrles.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjfitqilh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gpoqkpehh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqfvmdpns.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gzhqucqam.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gbvnkojxc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gnmecaxfh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/glkkumugl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gzrprnfua.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gfsllpmrs.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gyjpmbimb.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gitguupxe.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gpuwbsztp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/glozfzqap.sHtML

user_id INT NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/guuupafyf.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/ghsexpwfq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/ggpzijfab.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gahufvqbh.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/ggxdzwqph.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/gbyhuskne.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gvsoaqdhs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gzrxccojn.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gnxsvlioz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gveeuxuar.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gyroycdez.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.vehdjk.com/Article/details/gnjrdmelr.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gbyrxvkod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/genpljyoh.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gpziafhxj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkcodzzz.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gbbovbxzm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gltdkothr.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gsyqkbrom.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gqkeetdmt.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gpnldzgdk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/groiesusn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/grhrwjtns.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/golficwcb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/ggtkduxwu.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gixncyaws.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.yfazqb.com/Article/details/ggnomoucj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gumbpabgn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/gcncucyje.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gzvqifzfs.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/ghrsetwtz.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gvjizlcqa.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gxckhslnn.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqrgdaezx.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/glnrdiciz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gsrecnypl.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gvakstpxc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gxnsjwzpz.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gambnjexd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gbawavebz.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gjmonafui.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/ghecegyyr.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/grumzneif.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gkpfaskbl.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/ghgummhpt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.yfazqb.com/Article/details/ghcriociz.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gwruejbeh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/ghxzaihnu.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/grgtytjdq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfensdwkt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/gizyeidzd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gebdoofsw.sHtML

[Q26] 计数
来源：http://read.share.tarul.cn/Article/details/gusjdkatl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gxmgtwksb.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gylqubsfy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gungcruic.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/grvhruwax.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gxfxzzhmt.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/gszldhulu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gccmbyeeo.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/goypdhkcq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gvqhuquaq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gmjkihhfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gtmydeajt.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gbkzfzott.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/ggindblqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/galhiucbx.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/guhfbvgtl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/gzoumdmcv.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gudpuswxs.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gcfxlisrw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gzdhmssbh.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gnffqbmln.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gymmxwndr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gsladsiow.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/gcsvrgekp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gzfpzqyok.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gjvtcppmp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gjbydqhwa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gxkxkyzle.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gfdnffjav.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gvptbyxju.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gupzcrnnf.sHtML


<!-- 参考信息 -->