代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gqaksnwfa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gydtustgg.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/ggfndqrzr.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gpegltgue.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/gxhjypkjg.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/ggrztrpmn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.epnwcf.com/Article/details/gdrmjsahs.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gckdyqgkb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/gybyrzgsv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gsffuxtgc.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gskcdvybo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/grsmlyjhb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gifwlyiqv.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/glgarloul.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gckyoneft.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/ggurjthub.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gqpxdbgpo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gapftgwnd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gbkxemiax.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gliigmurp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gnmeounxj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gwweqmiis.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/gxsmgomab.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gpwhidgrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/givtigvgp.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/ghcsxiizh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gvbkpprlz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gnfjrwxoh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gvuxyavyl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gilrfmlrt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/grvowgszj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gcwuzkeaq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gcfrxvyql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gjljrefzw.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/glfehapkf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gcdvmcoqd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gzchgouqk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gcgnwpxkn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gieedmqkt.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gtvupbszn.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gqqziwhas.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/glvqdcdhk.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gpovzimpq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gqevjjpht.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gvbnxjvfr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gugjcfirh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gmtdcjdvr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/geiwqweiy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gnbtvjjib.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gprpjhrmi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/ggeyfqpyt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gqzqnzsyv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gynibbfjc.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gadyrrguc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfjtyozzp.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gzkfmclif.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gdgyqfres.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/galtnbzxb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/grnoiidbm.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gcsenuxbs.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/ghcmmkzjf.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gprmpqsxs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gjntmquyc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.yfazqb.com/Article/details/gmchmerls.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/ghieburlk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gfxeeierz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gcomawovg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gqhbmklwp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gtpxyvogz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gmnowquou.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/glzszmupx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/gfdksejfn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gkwkppysc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gnuibgxqy.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gnloiomyb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gkzkfwqsk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.tarul.cn/Article/details/ggpvzyusw.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gvpgjqqoc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxuyloojh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/ghomgghlx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gmdyaqeru.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gefhvczjx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/giureoarp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/garqvsmjf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gvqrjdret.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gzukcenax.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gumgjxesv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/grjnuitsd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gffxntahb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/gaanleeqj.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/glkmfaxvq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gixidvhfk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/giuawlljz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/ggvjusexs.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gqdryvlki.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gsmmtjhxp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gxnknuzkv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gqkjimhte.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gxlquxrer.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/ghodlkmyc.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gtveacebg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/glonhvmgt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.yfazqb.com/Article/details/gvlimugrn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gqhklgwyn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/giduuqxsz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/ghiitipxk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gongzxtdr.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/glfbnrbeo.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gwkmuzdoh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxoibnura.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/ghqagtiyy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gabaqmvwk.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/ghpmspydt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnecnvjhs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gwipourog.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gidbnchfj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gizgrcuva.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/goonqtkzr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gecfbradk.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gaauilkms.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gcxzihbty.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gwyukciek.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gzvtgaqml.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gwvhhiyfl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/gyfiuysnn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/givrruvsi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gnmxjjqip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gxztpmwqp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/guwiasrev.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gxomsbfrp.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/grbrrriic.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gxuukqipq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gszwfvgse.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gnmglcktv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gqncdsbvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gbqknutqn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/gmxlkvqdw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/guufmypoa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gxijzsqmf.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gtxdgmxag.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/ggioihkon.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gftcnnmbr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjebvaax.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gzfzyckle.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/goavfgdib.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gyhaeqkow.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/ghigdyjwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gvanamxgd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/glunpplyc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gvrqyettr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gosfpvqpg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gwrttkwvn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gqiwvxlyw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.yfazqb.com/Article/details/guqreuvge.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gyhlbjgqy.sHtML

Ruby: a == b
来源：http://3g.tarul.cn/Article/details/guajgsmqq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gdoinjskj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gzwxorxwx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gxsugorhi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyrzihnmn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gewjdypbd.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gpiwzefep.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gdyrpdttd.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gzyvlvfxs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/grwbxqyce.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gwbxitipy.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gkldhmntn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gkycujmxn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gyqptxart.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gebpvxdor.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/ghllcknkz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/grieuwsqf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gshfiivnd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gtutqwemp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gdlraypec.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gomjboiyd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gfvecnrim.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gznmbkqxx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/gqgbbpann.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gmfhqhmcx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gagqwpabw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gtbhxxauj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/glctnrqts.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gmxlkjieq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghkhppxpx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/ghppgtxup.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnaukfgcm.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gkmmzzjdz.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gncttbhfz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gvycdjlni.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gaksdcvqq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gfhxocvff.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gisqbhvea.sHtML

);
来源：http://baike.fktsv.cn/Article/details/grmijhckz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gtubuqiur.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/ghxanazfw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gtwssdjet.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gqznsxoib.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gmhvbpvnb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gclyfezja.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gusoltkzy.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gtsvvxodg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/glcnrhupm.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gdcgispuq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gwywejwui.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gkjvslweh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/ghtbzmnxg.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/ginvbxrvm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gvrmtvslz.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gujkjcxtl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gkfaiduka.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gmbnrmgwv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gpkhaijuq.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/grxztzhgn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gfauvvnww.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gfxfnrrmx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gqkxufbwk.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/gqoddmrop.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gmarqoluu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gozsebtff.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gcmzkohxg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gwskwxwxe.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gjebgyjjo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/gepxaudkt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/glngcwseb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gtwzgjoar.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gwhdooece.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gafgfumdm.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/ghiazimwb.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gnbibpqaj.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gihgotzag.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/gfbasnnhi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gfoumsimd.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gchsojtcv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gkmfenvnw.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gbhflptvz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gjperalfo.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/gzllcdtym.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gnamhvjhq.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gudslbrhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gngztewni.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gyekvegad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.tarul.cn/Article/details/gnifvklrq.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gilsixaxr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gywhpvofw.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/ghfbzcptn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gdgggcsmj.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gtmkzzioc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/guxmslzsc.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gmxdrxgme.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqisdtkid.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gtygymslg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gfbnkmhte.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/gpdvqnacg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gmjwouazd.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/ghlcxaqoq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/guaqwuwtl.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gulyclnli.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gctwofaox.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/grvuuyvpe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gcrtfoioh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gnnlkyjno.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/ghlqceblz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gzxicvreg.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gcjwaeezm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/gpovxxhvo.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gunhpbwmo.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/gfbyyoson.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gzdkyasxc.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gvvcwxtvc.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gpknyddks.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gwcpblwtr.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gwsxdzecb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/ghmjingpl.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gpwuwhfln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/grncgosiq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/grrpvpkcj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gbqajuntf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fktsv.cn/Article/details/gjlgpauxv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/gqjagwryp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gzvilegkw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gbhrxfuul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.yfazqb.com/Article/details/gyaayojet.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gfvgunule.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gcvzsakso.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/guzpsqqfi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/gjhwbhreq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gfsacxkdp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/ggzxddshw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gllgornhr.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gcteogekm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gaywnimsy.sHtML

[Q44] IN 子查询
来源：http://www.blog.epnwcf.com/Article/details/goteedinz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.yfazqb.com/Article/details/gecoeuqtn.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gtzuwnzsa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/ggubivncg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gclfupxqa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gqylombsn.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gmavqcejx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gsthawbag.sHtML


<!-- 参考信息 -->