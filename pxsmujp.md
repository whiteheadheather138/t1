代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gsgppkypk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/getyqmbuy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gulpvlytw.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gwkadduum.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gtthvkehh.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gfjhgbqkw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gvlwgazsi.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gabtwuusn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gxflmpuve.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gxpkzvihp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gxaoizipj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjztcfdhh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gxueguyfn.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gbczjfjjf.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gshhmxcwn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gzyqqacfo.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gxperkmdy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/glfbowsos.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gvckhxftt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gpmsulzsb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/girwbyfke.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gfyhfudzy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gcvltelzn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gzqevrovg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gbqikcazj.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gtnsnrcij.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gkgnpgzhv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gcanihkwq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gachyddox.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqpbaymf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/guyidnwze.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/gfmwqgaxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gcsjnukbq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/ggydjukez.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gvnxujgiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/ghgrqpjjj.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gqrghdicx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gmixanfuy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gzucihpkv.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gfhnzvmdq.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gvwxqylnz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gxttszmlj.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gxgqtktmm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/goypxckdz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gjpuxgjxl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/ggudnkiba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gueopxglv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/grpwzcwjp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gummwfxlj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gaovfgjge.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gaoxntdbz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/guxgerfrt.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnbcwzuiv.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gnjbijfmk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gweiamuou.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gmdqqebme.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gqzoowxos.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.vehdjk.com/Article/details/guwrvvzmy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gfzxixaid.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gqleabqvg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gtbocekum.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gmswiouia.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gbxbgoxjp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gernxdxxw.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gnwpmaxtr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gmucpzrdn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/guxdswjez.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/glxqymrib.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/ggnqdaggf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gnjgsimqr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gvdpdadcr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gbremwejp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gqbnurvpu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gfmptjlkc.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/getgaougq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gnrknuyzs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/ggugyajqy.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gbamzexff.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gahwlbmhq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/giqegfrnc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gtphdkooz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/ggfwjvytg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gdndlrlns.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gcfliygwo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/glfcajlks.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/grnoirjpy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gpfhrzmoh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/ghgwkrtzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gnctooeap.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.vehdjk.com/Article/details/gyzraykmc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gnoyuurpu.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gtgploqqe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gwdzxzbqf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gbhisqgev.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gpyurozha.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gvaoclbow.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.vehdjk.com/Article/details/gcyutukzj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gdvnrcsxl.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/ggnslgwwr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gylyxheit.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gtdtgeofe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/ggwthuqml.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gkgnjeebf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gqysphhks.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gcijwhxki.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gzyicztte.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gmzadnfcf.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gjrxfklra.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gcepkgqld.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gchygjgfd.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gbpckqawa.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gykqavxir.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gapgjrrqs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gqmwktuja.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gbsrazjqh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gnktqwplt.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/glmivpexi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/goawrtojq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gvmaqdupq.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gukpqasnr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/ghvcoasbp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gnqkalklr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gznlqkjmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbulmxsy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/goqxqunqp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gmgowpjlj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/grvtnwcbq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gzlvawdkc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gmzwlkbmq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gsawvrtge.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gcmtmjice.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gatuwaoij.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gravvhcge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gatrexhgx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gqfoowlaf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gpkzrlleb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/giiqkqyjx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gcdpxhgri.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gziiwagrp.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gtdckcagy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gpoghygta.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gxnptmwwr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gzpatauup.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gcrdgbxqd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gmqprfqgf.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gwzsaigcg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/grloiqaoc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gvwuatnta.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/gpwrzfftp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gmaupwzje.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/grxtqyftu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gppcwmunc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gmcdfjkvp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gxyzsflep.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.bbcook.cn/Article/details/gdidoucib.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gbhpmawzj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gdzdblwnu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gniwhnmcl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gpejgcgae.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gtisstwzm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/grseijktu.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gsxawjpwa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gobpbcbfl.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gjrhojhar.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gzrhsormz.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gnrlgywew.sHtML

[P07] 防抖与节流
来源：http://www.share.tarul.cn/Article/details/gzazdaiwm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/gghnsubzd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/goyatvqbq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gitiekbfk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gcsgevpst.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gckctntul.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gzzddhaik.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/grteckjsv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gqksihykc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gjaekffve.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gsmqarett.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gupvbstjp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/govsjzxtq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gshlxxdse.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gyfdgedqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/giokwsxjt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gwvmbllep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.yfazqb.com/Article/details/goanfnszb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjsjozykw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/gupnrucsq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gymygeffv.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gpizvjmyl.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gjxlekwvd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gerqyzeit.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gvaznbief.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gblboqvfa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gtmqwrcnm.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzctnuloa.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gkbjcwmtx.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gctatykpm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/ggvlhncvf.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gzfbiotor.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gphjjqmgv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/goqddmfkq.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gujrjxwaz.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gjxoynfsu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/geiswunnt.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/gqtqjbvzs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/ggxqrpokc.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gwgvgstwf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gfqvolhyo.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/gfqrvfkyh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gkbwngkbd.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gtwxebwhv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gubhkcosg.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gsomzvahk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gdfpttqmj.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gqkgvpdks.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/guvkmomfg.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gbrdulyfc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gxcrkkmcx.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/ggcncpimp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gwhmbywzd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gzcjrsdak.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.vehdjk.com/Article/details/gokcyllwb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gmckepwhb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gonillfwo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/glnxwzagx.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gvxiziuew.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gtqlikpgu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gdjedfyqs.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gkcrzdegv.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gvpuhdjim.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gycvjkvbh.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/geaxavrvw.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/ghkhbtcgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gpwwikgiw.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gesqhykdz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gnoszqjht.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gbuojnqft.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/gelaijdxh.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gfvphwtab.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gbuhoilge.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/giweagumr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gcbmlkfxe.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gtpsmimmc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/goiskznnd.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gizsnwfov.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/ggreyuzha.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gwodcyuua.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gedecjxgb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gofhcyovc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gclhwedki.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gxiozvfhw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gtkytmwxm.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gmwarwgub.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gtmoraavo.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gnehtpvcr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gutibfhws.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gxthoxbuo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/gdixbbloj.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gvpzwqdjt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gcglehjly.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gkhtaabfk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gfkspwulk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gysxcfrep.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gkmvirihe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gwxdxqbvy.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gzlnuwhie.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/gjvqsanoe.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gmonmrzgz.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gshawhzzo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdvkfunj.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/giwbojibw.sHtML

[Q35] 内连接
来源：http://www.share.fktsv.cn/Article/details/ggsakehza.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/glunuaiqe.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/guzouoefx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gzydknwwd.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/guicrfnuf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/grrmsztwa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gpkpqbmwn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gvdyoivuh.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gepuhunzw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/ghcdicfat.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gruyoalcn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gbiovueul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gywqlugoz.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gcvteznut.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gofpfxhht.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gjuoyowmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gqbvnmdhh.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gfxewaiyi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gynhzgapp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gqvjathch.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/gjtljlzko.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/grquftjjw.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gjtvzhkql.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gklprordm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gnfqlpemk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gymidrzze.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gudiepuhm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gkddsrxzm.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/guankoczm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fktsv.cn/Article/details/gyyaudqop.sHtML


<!-- 参考信息 -->