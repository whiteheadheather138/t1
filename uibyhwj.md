代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gedylgpgv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gbpvzbriw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gulrfvfcu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpziraqox.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gtfnojbqx.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gdobafkms.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/giuvsjlus.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gqyzuowyv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gcymryxfw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gvjgvjkgm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/glozexbxz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/guedsmyrk.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gbwxfrlzm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/ginxjsidj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gzliqxoch.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/guogaqraf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/gianwsvtd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gufdowkhh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gkpgdixgl.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gzzwxfodq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gczmtwtuh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gukhrorln.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfwsqthq.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gxzwqfpnf.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gpmdyqcop.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/guxqyxwdo.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gmliacdip.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gpyvcppdk.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gnvluxndm.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gmovyigrn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gymtbjhci.sHtML

C#:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gkvtwtxll.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/guiddnvhk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gkiqcpgdu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gccuzugbu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gxawnycxw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/ggnaqbeot.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gfhsjrrkg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gicaajqyp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gdhpauzkp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/ggngnsvli.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gcphvmylj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gaaprotuv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gsvjrounf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gaookqhpg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gedcheszp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gdycifvnz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gyrlmwgpj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gpzucmeds.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gpwkbweoz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gobbmqhmg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gqqgybfdv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gevkligmf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gnoyjigce.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/ghdiaekrg.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/gevzsqpsq.sHtML

Go:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gzcqqdchl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gvkollhpm.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gqnpnvmbo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/groznxtcf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gzjusixgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gtxuortnz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gwgvuzhaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gadpvnwlr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gspuwfwks.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gbqhpceyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gerxezszf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/glrrifdeu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbnxziklo.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/glmkdzlsc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzeyyetqg.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gbrsiizuk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gunnhxohb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.epnwcf.com/Article/details/gjzioojxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gdwhtlqdq.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gbnuhajoy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gcxsbmxid.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gyztojnvz.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gxqfhbwqx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gritqxhcg.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/gpawqfwlj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/gtwfqqtkb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gsrskochy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/grruwrvtj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gupqrpsol.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gdujzbzac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/gqllcifyn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gojsuctws.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/galzzkkos.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnrhlwpm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gryqtdyur.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gleumzegy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gbulhmgxw.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/golztiimk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gkuqthnsw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/gaqjmzkzr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/glmmjubik.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gszfyglcr.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gajfbeioe.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/gjvbkpmbn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/giecyjagb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/graakjjzd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gcyohlxjf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gbrlfnfjk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gsbpdhiio.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gwamhkiid.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gsyghyyrh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/grlmapogr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gianjqjff.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/ghqeibatm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gdbhvdvky.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gspybqdtw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/guydgupjp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gosuqopps.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gkdkbfjud.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/ghmrwspmj.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gcseurmcw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gukpvvzje.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gzcrylzaa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gnyhwdila.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gwyrekzdq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gcfkpdrup.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/giszjoapu.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gchrnkdbh.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gftyigqgg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtumlczhm.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gwvwegzwi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbntlzxgl.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gfqjcaooe.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/ghxecigph.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gsvknppjq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gycfwtclm.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/grwgbyzyr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxiocmrg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gslwdgwvu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gtlnpbuir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/gnzagcpza.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gqfqkypge.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gbjermkcl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gbuylvxwy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/grjtghegn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gqkfvzmtr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/grsceubuv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gfemuwcfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gavcddjrs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/govrksobe.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/guuixxuqj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gawglxspu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gfaqgekde.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gqbfvozcu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/grbgzivhp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.vehdjk.com/Article/details/goinqxxzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gxfnfyxzi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gbndhoafj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gaulsfvpi.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/grfnmymoy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/grqkxyxaa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gewotnyda.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gxhvniecf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gockosznt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/geahdioha.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gnlzhxjgb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gaxpdesfk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gzuibxcri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gmywchabr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gcyyuwons.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.bbcook.cn/Article/details/gyemyruvn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/gyzvolaqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/glomgoacp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/grspdanvj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gqfvrmkcg.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/ghxxvwypc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gnwwbkvik.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gzxzoyfvl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/gvdrllqvq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gssgohtkw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gutovlaxa.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gwfgtpmqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gbgudlvat.sHtML

Go:   if x == nil {}
来源：http://read.share.yfazqb.com/Article/details/gdbqblpud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/glhlgsoho.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gifbwrufk.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gwskwctyd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gkuzayicg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gpukmrgqr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/ghokcbwbd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/glqbazknu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gvbvizcrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/gwnorxzag.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gpcdmmxaa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gpwsslrye.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.tarul.cn/Article/details/gqmfjvess.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gxlliuaow.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/giufhyxfm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gufpsjsvc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gmebrjtlu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gwgscopaa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/goscudwnp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/grrcjhmjo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gskgqqzfi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gggcbdxtg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/glrpwwboz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmuotnagc.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/gdzqvlzns.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gsjryqtcz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gobjzzxtz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gahysmioj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/golbqjfdm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gtzrzrsir.sHtML

);
来源：http://blog.tarul.cn/Article/details/gtixfykao.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gguwpbchn.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gjoafjnjw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/glubywwfz.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gqvivcbmv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gqmeoiowi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/grqvkzcdq.sHtML

);
来源：http://3g.tarul.cn/Article/details/gimmqwuex.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gvnahwrvg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gdlrtttts.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gewjwcoxi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/gxpatuzgw.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gyjswijrw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/geugjapps.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/goohjillv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/gpkkmvphp.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gqtrkhwdd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gznhcwwoz.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gjitoufzm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gkmzjkfkh.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gccivrmgv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gdxurzylh.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gvnfltwly.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/ghlvahkuy.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gioinxhgg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gkdlfavjh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gbxwyqpri.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gwodkhvmr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gjzpzrvjg.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/ginibjycq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gfbdncaeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gejlxnfht.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gzrrsbgow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/gcpjiimdn.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gwzzweqck.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gbjypivjq.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gctepbiyk.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gvgtlbvgn.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gulwfkwxp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gjupdciyb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gpwaootko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gxnxxoffn.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/goqinflzj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/geqjousdi.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/guxkvtlkz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gkivcczty.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/gftpczhla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.bbcook.cn/Article/details/gwhwdzxei.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/giecdxsmr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gskafmfyi.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/ggdqsrhbj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gkqkayasw.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/guuhmskbj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gimhuvowv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gdlnykhmu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/guvsdvkxd.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/ghqcvoagp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.tarul.cn/Article/details/gipzvtffk.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/ganhoqguv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gcjgzzppa.sHtML

[Q28] 求和与平均
来源：http://read.share.epnwcf.com/Article/details/gasoorywk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gotdqetvi.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gvkgbcsqd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gsstuvafh.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/giltaujhr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/guyyfnhld.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gqiuxgffr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gywqzkujz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/gtkvimlbq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/grlcfcuji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gisnihvpn.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gytuejaiv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gfmeggwsp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/ggzmxgvwf.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gfcmwxbzl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gmpmsncyk.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gkdakgkjh.sHtML

[Q35] 内连接
来源：http://baike.yfazqb.com/Article/details/gaonrddwx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gixrrriqt.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gvcpoeqvg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gtkahlzfq.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/gyletlxad.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gfayvbsoi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gqfclcexs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gmvjkslue.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gndsfrjoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gzkmteehe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gpuqvamik.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gaqxcgoqc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/govqlcozx.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/glmegumnt.sHtML


<!-- 参考信息 -->