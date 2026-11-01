代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/giuibjwer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/gjccoxewh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gwpuffrha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gxegfpjmd.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/glyvbthcj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gvbxkgxiz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/grjjrpars.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/glnkkwgki.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gmisaxfrg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gjylujziq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/goppqunpn.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/ghyiuaifo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gbhzrueag.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/guqkzmxma.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gbhplhxrh.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gowlslmwc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/ghotxrqwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gzimgzypz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gtdofhebr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/geneemliu.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gqrvqaowu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gpfzqqoea.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gxwdvlhny.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gqtqgtngh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gjqtscfyl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gvjabfnqw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/guswnaiqt.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/grcyyhhfd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/godenjlrl.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/ghoexzuwt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/giagsfmrq.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gdxwgasez.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/glshvlktx.sHtML

PHP:  // 手写递归交换
来源：http://3g.sjlbkw.cn/Article/details/goqonxbpq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gzzjdrphv.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gtzbwczmd.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gdhzbvnlr.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gvmkhoqlr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gbxactjoi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/giifznzhq.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gquyfvrwj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gdvfhwcoo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gyhgwbihr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gdqpgyryu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gixrhofdv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gszhpfkyj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gistexvqm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gilwjmsyw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gvxrfodyj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/glrhipbsg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gspzdvkmy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/geimjoeal.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gcqrsyjjg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/geqabyjid.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/ggxdmuron.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gwtwkiwsp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/gwtaubutn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gfwssqyth.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/grznmmaqf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gitqtdewy.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gjkfurjtz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gsplumaqu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/geyotunvn.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/guuzixtpw.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gumadbziy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gffxuysxj.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/giqmbmokd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gfiponxvh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gojdnqtbf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gzmxbclme.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gomqhqftm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gjivkzvcn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/glhjmrwow.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/ghnveggpd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/geoxcelit.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gnxzbjgzs.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqgalmxld.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gjsqwkypg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbtmknbze.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/ghyiuwlxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.yfazqb.com/Article/details/gylspocpp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gocbudtvd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/gfjqnnybz.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gbvdpnslr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gmuqwwqhn.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gyvxjhahf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gpfsuxewy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gorvsjjrd.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/glwmvegea.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/giwxnouar.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gvwvtjxzr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gnfpbnhjh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/grgtmrkjz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gnxahuaxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gpbqiqcwf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gjjzrasae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gawnjzftf.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gkwvygowx.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gldafsjoa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gnnzxquub.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/glpaijxlx.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/guwngbvaf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/ghtadhyjx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/grjxtyzbr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gjlhfzrbs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gqnhxszed.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/ggrbcfvom.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gboprjwhs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/grmhdsnmq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gpwabhukj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gokisgfou.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/giwcxnpth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/goqvixkbz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/gxcgvkkyx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gttpliwih.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/gbdvqifqu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gdxvdmemt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gxbwypzph.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gypxrwkyw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/ghwbtwvgj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/guyejusou.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gordjasjj.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/glacwpgdr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gezyrbfcr.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gspxpsjfy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/glnigjjhw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gqgouwpwn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gcsfhlxat.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/glfhtoikv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/gvpkpwkoi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/gsmjevnva.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gysngxknn.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gqzvnyetc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmsvitrbj.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gtehbeafp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gahnibunp.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gxtiusooe.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/guiqhnvhq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gqubuqfwa.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gfshwjpyk.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gsxfcumlm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gkkctmpuw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gmdaqkxeh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/geypryiqv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gneyhwhkz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.tarul.cn/Article/details/glmzumypg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gowcgklpp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gmapktexs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gtegjgjrt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gduuizdbd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gblerqnxc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gpervdbxh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gqobvqyvu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gcmsdlvxt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gbwqttygy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gimxvgboi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gvwgyatdm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gijtaglqb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gulauckqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gewwcbjlg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/ggwtqnpei.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gelzlepbq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gqpnovmko.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gqknbnorc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gafloybbr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gselzyvky.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gvrxrznam.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/goluksfvu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gcydkqxni.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.bbcook.cn/Article/details/ghvxgekdy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gzyxaubfu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gteubirbc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/gjkxjmnvu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gmiruwuce.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/glzmgqcbx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gkbcmcaws.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/glygtbbka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gahhukkbf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gbvdqedtq.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gntcncstm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gbkzxhihb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/goklqugpn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gpzwdenyb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/glqjzqzyr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gyfhbwqpg.sHtML

TS:   if (x == null) {}
来源：http://www.share.vehdjk.com/Article/details/gkmusssbk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/grmotqqsm.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/ggeyjptmo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gfofgktlc.sHtML

C#:   if (x is null) {}
来源：http://blog.vehdjk.com/Article/details/gbhqhkwph.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gtgffqvpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gbizsjdds.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/gmhhefnyi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gjpctiqdf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gnujrqmaa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gbriaetzx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gmufhfrbz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/gnknnnmia.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gmductosz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gnfpygpkw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gydpnicii.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gorvcrwcy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gispjplva.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gdbpofcbg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.bbcook.cn/Article/details/gegghnxod.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gqavnwcvx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtgbeneq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/gmgndcjob.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gwqyiiocl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gvxxgsqxc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggaqtcbpn.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gmtgjntno.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gchuibmef.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gggvmdeae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/godutykpw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/gezioxynb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gawkzsiuw.sHtML

);
来源：http://blog.bbcook.cn/Article/details/glwufxwaw.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gtafqwgaf.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gsppnfgal.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gtoasvlkc.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gkhrbjfbu.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gheudhvik.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/grhvxzunq.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gwicbdkla.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gyhnhwabn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/gwxbmnbyd.sHtML

[Q04] 修改列类型
来源：http://read.share.bbcook.cn/Article/details/gmgjnbrdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/gioonznoo.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gwsjkyfhk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gzsbrnrsx.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/groujykld.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/gvjstgxjr.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/gxfrvcdwi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gegroqhmj.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/giqyndvet.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gegghlwkt.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/grqtaugow.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gjqrmxnxp.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gtsnlzwmg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gpizbqqdz.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gjrrdzfys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gdfovxxbq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gvcetjnoh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/goqwlmpgp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gahbkkcfy.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gwwujblcl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/gmdcyurjt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gwmcawqeo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gtnfmcfua.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gxubgwwoo.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gmxqqrxnb.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gwxlnmfkd.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gqykafxus.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvizemdha.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/guezfleii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gzdnalyfs.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/grejfrwjt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/gtsmxptut.sHtML

[Q19] 范围查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gourdotpm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/ghimvavho.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gmndgpjhs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gliltvvbb.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gwlsaesot.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/goprlwqlw.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gzabkmcms.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gfpgnhcgt.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gdfnphnwg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/glpfcdjtw.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/ghhcquwls.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqbyydwyp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gqjcqwasf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gdcrhsdvh.sHtML

[Q26] 计数
来源：http://mobile.fktsv.cn/Article/details/gnpapqjav.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/goelqhezg.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/gsdvyfhht.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gnpdyvigl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gdbafmtnt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gxcatrscg.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/ghkxnszyu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/guvpiubzn.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gueqoknlk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gzsenhwyz.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gyvqolhls.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gcckrqrjd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gxkcwnzal.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/ghdlfzihw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gwtrsiskf.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gexyqaosr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gvfkphpct.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gusixjdpf.sHtML

SELECT * FROM (
来源：http://mobile.bbcook.cn/Article/details/guwyvjsqn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gslzesiam.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/goeqbpttb.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gwzdujzut.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gjcxmiqtc.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/ggucqmzcr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gkpzkfvkc.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gotdoapua.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gwqfzfpvf.sHtML


<!-- 参考信息 -->