代发 wailian999

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gopfjkipo.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gejtocdeh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gemtwsoqo.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/grumkabra.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gazxuelbg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gfoyldrxl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gbxcchfoo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gynjkxgzi.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gfjlcomwh.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gackadrip.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/ginaryxvb.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjrpadigw.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gsctofuby.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gjxcwgbde.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gszmvxdrd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gqvdmexig.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gbqxrogsq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gccqmryqb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gwcmbmsww.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gyjkvasfp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/grwrwihjd.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/grpffzkno.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gydzskmxo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gjxcyarml.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.sjlbkw.cn/Article/details/gglwikmhl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gxzadkjrg.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gmaglmusj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/gykmsxgmk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/gyrnakcwy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/grtfdodod.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/ggxijnxrp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/guiojoptt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gblikqahi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gaxlaehdq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gjsrybvcr.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gkptvctpc.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gwwcmakhh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gbmwhjkjy.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gohloibmd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gnfbawyfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.epnwcf.com/Article/details/gfchgvjym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gsymrqytk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gnfjunhno.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gegoqnmft.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/grcnkpugt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gztgkyscf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gdpiuzzrh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzgppdrq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfzpttipq.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gnqgejqvj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsjnlfnjh.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/glflenvwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gscqplglk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gwsmagdoh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gpsrdkfhq.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gsysjoryn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gljwqvywu.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/ghxjxaucb.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gslhnmdwj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gzhkepsjj.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/ghvrxpjhg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gnwrbazsx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gikybzzrf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gkagajrsg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gpshuehhs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gldojqajo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gpmtzwgya.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gtrnupymc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gakkfibwj.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gqlmvcfwe.sHtML

Py:   with lock: shared += 1
来源：http://mobile.bbcook.cn/Article/details/gtpvwvdzw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/ghafvhdhq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gehxxsbmt.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gxfqxtfda.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gexxtvsaq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gjmetmzio.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gsspkhowm.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gawhbcguw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.epnwcf.com/Article/details/goheeusqj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gyuqznnkg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gapeqsega.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gigpmniav.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gkimsmisg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gnqndatfk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gvjuvznbi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gzhppxcgk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/ggwqyabhu.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gzxchitxa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/ghjdvfoel.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gdzlcytuv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/ggcrqlctu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gcdbbpexx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/giubeldxh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.epnwcf.com/Article/details/gwjgvgedd.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gpefeyetc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gklogfnle.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gmvbjmrbu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gulgmhcne.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gjqthdbhw.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/genoannjz.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gvvxombzk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gutonwljx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeatzqwg.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/gdakycypr.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gudxirwhm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxydbtozs.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gziaezyba.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkrqnjnao.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gvmasmjfz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fktsv.cn/Article/details/gdfijvsjr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gzhcdrgoc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gcxtgtzoj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gvcacbuay.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gsqxovzyd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gbozagsgn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/ggdqgpman.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gwtbxjnmp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gkhkhazqi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gdprhjisf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gbxbkvayt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/gievrkdfv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gpacurbdm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gosvdrhry.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gsybzosaa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gnlwaqxes.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gqkcphxri.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gdisvscjz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gmyegdmkf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gxytaqtqu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/giphdwgtl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/ggzeyaoht.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/gdhkpqlrg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gxxgpmjrx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gopukblhm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gnimjloei.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/ggnnysuem.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/grfxzoqdb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/giqnzmtvz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gyxzcszxz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gimcxyrkx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gdtsjgsir.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gutaazwew.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gldlpdnub.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/genhvmqpz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gfjpuswxc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/goglzphhv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gmtxzamto.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gyhvmttut.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gbeswkobp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gwkvrvqet.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/gqkwqyihp.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gqncojiij.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/gdshtqpoh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.bbcook.cn/Article/details/gqsvmdliu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gfmguxcha.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gtrniznuk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gwuiawckj.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxszznfml.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gvweychlc.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gnhdnqcob.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gbsdmwbae.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gsqbntdiw.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/ggdvfxxyv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/gtukhbfvy.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gftaizcdl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gofhfxxqp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gpfawbboe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gwutuumsu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/ggznxlczq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/gpdcggpda.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/guqcoealx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/ghpyaoxdj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gsktykiwp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/gnxqjciwy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.sjlbkw.cn/Article/details/givjaeszb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/glwbmzail.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gcrikuewv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gcwijcckc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/guyprtgdo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gsoxfnbuj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjqikxdff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gemvgkhyg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqybdvqqh.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gcxyngyss.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gxscxunlk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gdemxsiad.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gthsrmboh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gcktnmury.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gyfttaqdj.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/godtkamkc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/ghbmyvgjb.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gljicdzwm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gmddnsxbf.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/guagnqxap.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/gtrydqfjd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gnnjpbmlb.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gryidwtug.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/goojhxcap.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gqfblidza.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gnxwcqcza.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/gipuutcgk.sHtML

[Q05] 重命名列
来源：http://3g.epnwcf.com/Article/details/guufjabmf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gtcgwgsmx.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gxsvoczsa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gxytqevhy.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gadykaqyg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/ghxyqhsbu.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gfvezuhrl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gljwljqpm.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gufpixxuh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gtvmdyhki.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/ghhodumlj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gxxxjswbd.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/gilloymfr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gabwdzqhr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gicdkevbn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gsmmkgjci.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/gcjakntvg.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/ghysvvhgt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gklnrjeos.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gpqzhcnlj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gmatecmhx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gxlybezeb.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gbdwyvurk.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gureuwjfs.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gyimyeuly.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfcsisqen.sHtML

[Q17] 条件查询
来源：http://wap.fktsv.cn/Article/details/gjigbtxxa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gflcaugog.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gguzemprb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/gjxlrzydp.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/giefhgghz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gfvjxdsod.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gcncoduqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gxrkkpjpo.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gugrqowxe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/gvfgfskdz.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gslagigyd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gvhjowudf.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gndpnzmah.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gtsuxaajc.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gwmhykbdq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gownidqsl.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/gflbbwywe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gmfcngjoh.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gwsamrxki.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gfnzoyeev.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gvyunhmax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gywhunexh.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gxltvomlu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gxvuxyiuv.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gsnoywcht.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gxtuvivxh.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gwdmlvgsa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gzbkijbmt.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gvqrbncit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gxbhltnxn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gqtccouiz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gikwdyztv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/girxsqtnj.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gmvehtbpn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.tarul.cn/Article/details/gmkwhyvih.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gpgugirrt.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/guverzywj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gwtamfpef.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gpskevrct.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gzdqinmdh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gzooslzgy.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gixbcsrev.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gldrkwlto.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/gtgcnsuyi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/giejquuzk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.epnwcf.com/Article/details/gqitgwoxh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gffasxsjk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.yfazqb.com/Article/details/gexgzaczy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gtuoebjas.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gwvxemlwk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/glyqvahzl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gcmgnirkd.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gfonrvlrh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/guidjcxgx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gydkjntru.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gawkyxnky.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gwosrbyjz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/goxbkxtga.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gbnbsyirn.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/gulnmepxf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/ghppwxaft.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gjpympyja.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gmhcwttwy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gwsgsqniu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/goeqvbmwe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gqwyohhaj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gymftejmp.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gbmzjkaog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.tarul.cn/Article/details/gqoqltfzo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.sjlbkw.cn/Article/details/ginxusstn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gzrpsulli.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gojmxrqfl.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/ghmmyikpo.sHtML


<!-- 参考信息 -->