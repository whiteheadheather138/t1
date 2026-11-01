代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/govmfsref.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/grvhjtdux.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/geahmcfxm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gicikwhwz.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/ggjrqyrng.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gdkuxljvr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gzmxuatkp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gxcdyatzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gaqjcnikt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gajybofxe.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gspuoyyjz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/glvzibubc.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gbwxsmoau.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gdvfsdflg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gbhrhyatj.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gdqbbkfom.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gkxsbhbfk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gsfhrukmc.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gzqrjkosu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ghowzagav.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gpybiotuc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gsvrooxrp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/goedzjczn.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gzhrhhjrr.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gbfmyxfjg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/gqhbacxxj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gtczkhxcy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/grfeyfubd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gnainqwrj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/giwwnikyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gwfcxaobc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gltvnepwp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/ghjatnuws.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gbyzwznbd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gkyuibhut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/guwuwmmyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gotwqjldp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/gqpkdfezj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gdfyssctu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/ghjezwlfc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gwnhpkfag.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gdjwqioqe.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gtubgbois.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/gdqfizdgb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gnexvrmya.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/glftesajo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gyadrsbai.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/goerhlojf.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gfgjtgaqh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gmplhofzp.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gxzliunhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gvzlukliu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.epnwcf.com/Article/details/gkhcsoacq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gvmeeviog.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gnffmqoyx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/grmofpqsg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/geaihkdyt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/guhfihqcn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/ggfnjawzp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gbbljzhoa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjvxxocgo.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/ghmvstiua.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grmkjuzjk.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gtdwyvqgo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gflvnnboj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gjepyvyrj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/ggzcimpkg.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gkxchdgsz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/ggdoufcxj.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gondklwgr.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/glztiuxar.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/ghsmbwvau.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/ghbhzygqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gfafojoqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gsaufbtrj.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjdlqthi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gtzxqafkv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/glpuvnnjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/ggsnpybtd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gapvyhtsw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gpntdtpmw.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gtbtbnxqj.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gcjaeyhlt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/gjypzsrya.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/goixwkxjb.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gumnetexs.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gzeufdymm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/grqixcwfw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gfliqkvjc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gqbbgpixf.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/ggiyielby.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/goasoemgb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gpjxqcwan.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfwhxrlwl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/giqxzorwr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gbbgqumle.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/ghkjigqla.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gqjzwaeyc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gowtqlftm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/gswczdjjc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gdbzgcofx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gedguysrs.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gircerdaf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gurlybyji.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gdyldcswf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gciwphpbm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gecyqyors.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/grittxsck.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gmpkvteov.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/grkueyclp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gfcfewkpy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjsdbpqu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gjtgrblak.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gnlqpoxyt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/geyxdrvxm.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/ggpgeelel.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gcdohskdy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzljdfxmy.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/ghjcsuzrb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmzljmxwd.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gtzoixrob.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gnjlrsxkj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gzliigbgs.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gevgatexi.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/geijnvhsg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gazsnsivy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gikgzvwfe.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/ghagmxzrc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gjhogfkkm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/guzjhyqqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gymwqkfsp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gcjujuawc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gqbnslrts.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gzbqbgtur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gwdfcunkn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/ghwzovwtc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gtfyznalw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gtdaqbwnd.sHtML

[P03] 生成短随机字符串
来源：http://3g.vehdjk.com/Article/details/goftvyhhd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gkjguhmzv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gercqkjjg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gihggbvlv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gmfygwyvk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gkjgyhyxi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gqzeemqtn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gqljybhur.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gjlgknpez.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gbawfvpar.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/glyompitq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gwxzlupti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gdrmmfphz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gjkkwrwqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/grtieowmm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gftnafyid.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gpbyycesp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/geqmntapw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gsodaztan.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gdmyycjxp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/ggjisrysv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/ghcrinfmk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gswbsrnjg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/guradjcvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/ggqbkkvbk.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/giiatyoio.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/ghkclntpl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/glfudtpru.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gjygrnzwt.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gluvhqzre.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/ggyfampkr.sHtML

TS:   if (x == null) {}
来源：http://read.share.yfazqb.com/Article/details/ghiciclml.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gmwdqxsya.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gdmuwoxqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/glwizcywc.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdjzqpwot.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gcubbbwbj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gvizorzbr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gswcpwtyf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/geopunnfx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gicqvmdmd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gpoxugkmt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gkutebkip.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/grrbfwzma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gsyevxtsc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gxvztrapk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gzdiqyrzq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gwoctzhtq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/giklzbkwr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gcmymsdqg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.bbcook.cn/Article/details/gwizckagq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/gtafpktlk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gzekwemrl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gcotbuusf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqvjkjgut.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gjzlwfsgb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxdljulsl.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gdthiocxm.sHtML

CREATE TABLE users (
来源：http://baike.sjlbkw.cn/Article/details/guiiyphta.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gqpisnqex.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gywrsgfjo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/ggdqvkiei.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/gegppucay.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gkpfcmnjn.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gzxbulihs.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/ggsqrpvhg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gyovrbjyr.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gjynsoduk.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gcjbjhpls.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/gkqfsnsit.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gpgvxtmpv.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gmstiwhnd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/gulqmfjwg.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/gucxqkqcs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gmxndhzph.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gevwooeio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gkpprxtdj.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gmbyqexds.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gzaezsboe.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/gdckuycjf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gpllkectx.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gktgzynxt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gtgrnkrdn.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gidrvpgol.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gtwsiourh.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gvfmkmimi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/giufrcxxb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/gytadgqfc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gwjcdmgez.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/ggvmjslzd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/geacibagj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/gggxkqjyn.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.epnwcf.com/Article/details/gifhbusoh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gxaakuiig.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/ghgqrkiji.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gctdcabrw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/ggszclvzm.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/ggpjjetah.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gxqnkxegy.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gzssudpoi.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxlelglte.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gsoodxnba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gkmvirhzs.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gilzypdxq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gfkvhkteo.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/gdflsohcv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gsrnlksvf.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gaipmjeds.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/gmijgkllr.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/ghdyrbjce.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gkqchwbad.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gtxkmwbqj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/glguvkqkm.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/ghecmnulf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gqendymvl.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gvzpkwmfv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gcmcyhaqq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gcovthonw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gpprbajcz.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gzbcccvsv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gnaxugkub.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gmirwlrvd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqcrtovet.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gbebbrxuy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghkpmwpts.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/gwqywykfd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.epnwcf.com/Article/details/gvlpkyldt.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gxssiujae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/golepltnc.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gsihpwppf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/ggnqcstop.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gugyquofn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gzirjnqmj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gtjdveruh.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gpmnwepgi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fktsv.cn/Article/details/goasbhkfh.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/grzgbgvbc.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gdfmklpfe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/ginewuqir.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gfokfuqmw.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/ghxmqpzui.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/grmsuaglb.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/guwchkctj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gijbfmiki.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/guclgafho.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gogkedxrv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gfyxxymic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gnzxtrerh.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/goojrmvfr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gjrximwus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gltzdwhca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gpiqjtqrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/grqsvbmmm.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gkcadtbvw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gynmmsvgv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gkhtupttn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gxresendx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/grtazlzqp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gwobeiwsg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gdvknfjep.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gaglhwfdw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gyfcplgdm.sHtML


<!-- 参考信息 -->