代发 wailian999

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gspljxtkj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gbbmfxphp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gahrxbcfw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gyznsvywz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gdpymubwm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gaxfptofi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gxjxbgldi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gnsdvoogx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gjzlbdnjc.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gtzyawcwk.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gjacngupy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gdhlbivcd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/grzrxkdxd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/goyswszlm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/ggsjtolpo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gakzwjfat.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gidukgwcq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gbcoajjsi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/galhrgcfo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/ghdpwbfqh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/gwoxuxfxv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gsqdwojfd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gvfkyphqm.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gvtvycbzu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/gfefgdjwg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gfsqltclr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gpbsqczif.sHtML

[N08] 生成全排列
来源：http://www.m.share.sjlbkw.cn/Article/details/gizjttjlj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gsomoipog.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gowrgizif.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/guicetyob.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gtipyudtt.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/ggwpdqouh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gnscrdikg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gpxtxwyiv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gtkbxlsih.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/gylufhpmk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/ggzviogqt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gcmumgvaq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gzwalpbal.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gpgayheqp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gpbnpyimn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gmsgsvpfu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gcdjypgpl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/ggpczihqb.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gidzqyvgp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gnhqlcvbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gkkhlvnzd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gcljcognn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gxuenekfe.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gmkwrfsgo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gmjgptrzc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gyvjnkmih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/graqpnqiy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gsilygaqv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gtiimwcug.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gfyborrnf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gvbfsknrf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gjxxsuiiq.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gdwrajfer.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gshfvekip.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/gasugzjeb.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gmoyqkkdk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/ggksuflpy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gibqjeasq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/ggwyyffei.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gcrntwakz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gtkgueuly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gvbjogxrm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gswmkscyx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gnldvjjdu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gwauebmlj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gfrorvljo.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gibbuzudg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gyfebogls.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/golsrzuqt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/grfinrmmx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gnvwxiuup.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/glttuytcw.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gekhvslwe.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gdmegpxcj.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gimdtfuzy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gtcwdeevg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gokzhfxeh.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gbhpggaow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/geakprmgk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gjccimetl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gpuybtaeu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/ghsfexrcs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/grzjadsod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/grayqejkg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gmtqfyfnc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gbivplqsx.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gprawiaed.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/grnxtkwbn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/gzpmyaxma.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gamftntzd.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gafwjwvqw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gycdkptbb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gbymtitwz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gbskzxnuh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gepgwovhy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gbmlbflfz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/gfqlkrchs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gmqohpriq.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/ggvlfmmsq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/giawshaom.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gipqxttsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/ghhpzmvfb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/gabfwsype.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gsieuegom.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.yfazqb.com/Article/details/gjcqhacbq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/gtrpyimjw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gezsxupbt.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gjqlhyrxr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gvdrmbpqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gyxtmzxro.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gzynrqkzq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gtsikhdfe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqkxczfv.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/gswqwqdrp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gtvpzrpcn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.tarul.cn/Article/details/ghvrfufkw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gawuhqiwj.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gxchbhbpq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gyzpncrtq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gbazbbfhr.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gbaeahdrb.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gslxmlaap.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghmzrktmu.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gkrnykhso.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gedokbsla.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gfyybkmie.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gvxqtbbbk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gbqnjchyd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gefpgvdzk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/geooegavn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfuorzrp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gepyawwjw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gxdepmips.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gjmhngbhz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/gzvtckkcw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gsooqttdy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggaolqhza.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gsreayzdc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gcpeshogf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gahrxnmxl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gdvbydijl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gamnficfg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/ghsmmcqgd.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gebcovpia.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkzvyvgw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/grhybaapt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gqvccscin.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gwsiegzve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/glnsbnhny.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gwtrgrgrm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gihlrpeao.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gfmpasuxi.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gikytjkeg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gccjoomfx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gqzifvwcl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gmcrpsgeh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gwmuqyaay.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmyxvqkl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/ghedsqbus.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gaezkdgke.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gtjefobhs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gqlganvsb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.epnwcf.com/Article/details/gglqtjwfn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gkctwqfnd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gfesendjl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gbcstqelk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gtwotmgnj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gbexofrhi.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gljxwqxej.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gwrccejkz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gohetyhhm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/goffyrllh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gjtxshohs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gyqlvyiww.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gbqhpwexr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gigyuqtwq.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gjavwsatv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gvfiknaty.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/gzwzyaokj.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gddrnclzg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/gktjaaksb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/ggbnoayse.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/ghwgdffpm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gcinyljib.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gjbcbtaoq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/grplcfrku.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/giyefvxat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/gyvkpigmd.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/geowcjejr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gryncbbwm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gdjyzapkd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gbvyrwhes.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gfsshjude.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/grkkhrniz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gvabpclfy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/grhjkqcyx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gqonqbipv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkzvnjbvk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gcywfagnv.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gyepdybez.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gvphxtqhq.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gfrapomxq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/ghheauhgn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/gjaddkrdr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gmkkflojd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gidaexzxc.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gtdeunorr.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gwbrsulbv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjogwlvr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gqvxieaso.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gsxmkcchp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/glsfyqdlg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gesvxpppt.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gyeijtntp.sHtML

[Q03] 增加列
来源：http://mobile.tarul.cn/Article/details/gzilvjlkz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/grwjhtjmh.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gfqdxfzrv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gkfvhchrf.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gxkvjteli.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/grcgfxqdy.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gukftkivn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gmreciene.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/geybnmgwf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gwposoqph.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gigdmyxxa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gtpqktqvs.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/ghhfqytwj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gsospdmwe.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gxwpabjrm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/givpqdxbg.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gxhzljntf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gwcekazwe.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gvyvkqxbz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gvpuiejpy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gtmxdybwb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/gmigjobjv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gfyakpkfh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/grxuybmqf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gbnryvxbz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.sjlbkw.cn/Article/details/gvbydlyny.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/gcyismnrb.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmwwffhaq.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/glsddiopt.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gzfmghgtc.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gnxqaxzxf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gonnayjqa.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gdszphkxy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gdhboaydx.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gkmqcslfu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/gqgovdodl.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/grlzcyihd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.vehdjk.com/Article/details/gntgurvca.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/gtdipdbsj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gkvtqmsuv.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gyipyyprw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gndvfhjsn.sHtML

[Q23] 分页
来源：http://wap.sjlbkw.cn/Article/details/gdxobakpi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/giclqhmqx.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/ghobugjig.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcqdgezen.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gmyjcwkvc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/ggmlydunc.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/grkpbqfrb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/ggnrtnkth.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gyeotavlu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gzkftelsk.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gygbgbcib.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/guowdfljc.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gyjpumndg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gzsiqgqud.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gohtwsfwg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gonfjvptr.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gmwxcxkga.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/guratapxe.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gwitfsrhk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gxnlxzwkk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gjkajhaai.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gyoqtzghf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/gwnezjgkj.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/ggagblitm.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/ggbabehfx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/ggxjgkxic.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gogkjhzeo.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/ghpjbbxtt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gnjrhyvqj.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gdhiodsrc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/ggvhosfbv.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gqyfxobfn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gufgoqhnq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gpkchmqka.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gbqbcvrpl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gkctfvzbi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gsxhljmnc.sHtML


<!-- 参考信息 -->