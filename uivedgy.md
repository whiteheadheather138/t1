代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gpfralcpd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gjktfocfl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvziqbylc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gdhvtuyze.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gqdvhwvlx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gzulxqgzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gcbqoabxp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gesbvhggi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnomqbqbs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/ghixwdjpd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gttkaggqm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gnifyjbws.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gchdbyqos.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/glhcuyvxc.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gpzcgxgqu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gygxbiuad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gwtqumuyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gykqqhkfd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gdprrirzx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/geqfksnpv.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gkpzggkst.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gqmzrfaww.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gjhtxkaff.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gbgphcgfr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gxjcstzth.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gkikmyjfv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gnaybzrtj.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/gccaprjau.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gkklxafow.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gicmhqrdq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gednoeaeq.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gfryqdxkb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gswxwxcxv.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/gnegqbvjm.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gchfqyfci.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gdbhjhmgt.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gtoeqzpbs.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gerdcnmtz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gwcgffwqj.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gzipitpha.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gmxtxgekv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gmvufyoll.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/guvpvjiod.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gbdldqgod.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gqvwlmkst.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gcbfbzgzb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gibnnxcvr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gxbtblkqe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gvmfbuzae.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gevokrbae.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjqtfezr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gtifkchzd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/gwptmjpsf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gabzegged.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gizgmyeqx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/grgoqtzrm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gjgaqxnzy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gdvxpazyp.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gzbibmlpz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/grjpclfbq.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gbbujpzlu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gxeeirorc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gxooeiubo.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmwytbzm.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gubmkrkiv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gjmahndxy.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gkvidgbve.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gmuevyzvw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gzpzyrtzs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gilyyixci.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gvnrjxyll.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/ggrkauiwa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/greobkdyk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gayglkgfl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gncvezout.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gzztpcfer.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggukgytfk.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gbjcavnsl.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmhisfrwe.sHtML

[O01] 启动一个线程
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlalgqux.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gpebspfdg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/ghsjtcmjw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gimdbqcrx.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gypfintdh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/geutdvqpz.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/guvaxbsdt.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gndhxvonl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gzvpdmhoa.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/glyvnqfcm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/gafavbyhh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gpdntcdko.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/ggectnbnp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gyfbmxbjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gmlmtgjvg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/ggoovgcgd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/ggwnnnaeo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gukuftqpb.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gwbzaacgk.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/grzhsvrma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gbqtnnuuj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gttbhimjo.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gpovdxuya.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gagarnyju.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/gzwtnosmd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gclbtzhcl.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gegupzxgw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/ganasteks.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gkezpllwv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gfucctinb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gjjhoxuhd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzkngiuyn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gzijcycka.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/grgpnaudi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/ghvphoqyl.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/ghngidlbc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gckspgcyv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gkiujmezy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gdlacebno.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/geljsilcw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gnnpqcenu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gotvrkmwd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gzhyxdvlz.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gbyreeekj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gtkvkglhf.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gjoeuzjnh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/giokqifdr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/ghuwfadza.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gzuuobirr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gfzzxuzdj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/ghevgbrew.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/geemvgqog.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gkhlnmjbe.sHtML

C#:   Parallel.For
来源：http://wap.epnwcf.com/Article/details/gvabcxple.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gahekmvbp.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gzhmbxlfx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmxjittpv.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gjexbxuac.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gtclrwaxq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gtmaxqmuc.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gtthfnrlf.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gjfkgujto.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/gzfpuzwtf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gipxfnvmt.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/glrjxcxxl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gvmatxltj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gywrpwtcd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/ghmytqlaw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gzgtakcxf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gwqvmhsdf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gigehjckq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/gsdnyeeve.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/gxmmkmzcb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/ggdgebpyj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gsdhtxmxq.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gdnidgobc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/grmcsncvt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/guiycrfjd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gcrnirplj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gkpblqfuh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gbgutlprq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gvgabsfol.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gyjinbrbz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gslogerxl.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gynjazegd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/glvmgoyiv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gpxpixcwl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gkcspkygn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gogtbpecz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/gwgjulzpp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gmruebpge.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gogzljwan.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/gwyilonnd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gozehvmnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gqtnogznw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/gatsartiv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gyvlhitco.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gblzrkoqg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/ggrhfwjol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gfgyhvdxy.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gidxmbmbh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/guwkkneyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gkpskhzed.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gdrcxbqcd.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gzotydiuj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/guvombwoh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gajceopbf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/glkesqpkp.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gqcpvupxa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.sjlbkw.cn/Article/details/guwbzyclu.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/guawlzzac.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gvtghahrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gntjwtpvc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gjxjycalb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gqadvfmwz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gezkaoupf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/grzrrnjaf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/guxjzhirz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/gzongiceu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/giwjrdyfy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gfvggomvr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/geeblcolq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gnveuodic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/gxlzzzmgt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gkmakhayc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gaihwbmis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/guyfalvnf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gmhcqniso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gsrzqrdio.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gypvvjbju.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/grugxkmxp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdszcskdf.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/gqppfvvvx.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gvfcweqqk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gkaflweme.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gcshiqlcb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gjwvkecnl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/ggyvxqtyk.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gnpsvagiy.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/gmzwfmved.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/glgemcmbs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gzrvmoumn.sHtML

user_id INT NOT NULL,
来源：http://baike.yfazqb.com/Article/details/guevgqzos.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gvwzlnzrq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fktsv.cn/Article/details/gbpnukgwk.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gfleftogh.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gakzairyo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gkjeklumu.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gsarihxuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/geisorxsp.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gboqphyyw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gjrlkrerb.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gounwffzz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gmfrknnte.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gudoeyvoi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gnftvxvsf.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gxrbpcpix.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gqfluthfu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gfwsjufnt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gueegbewe.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gqyxmgtic.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gdomupeay.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gwolbpjpk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gplcfxfsv.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/gofoknqvd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.epnwcf.com/Article/details/gcabrfhif.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gceafbbkb.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/guoauqckp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gpnaaoixl.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.yfazqb.com/Article/details/glcqhzyre.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gywnsfkqb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gbrzumfkf.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/geczquhza.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gpkellddn.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/ghksgzwho.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gcpmwlzfq.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/ghjzsbxib.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/grfkjdwky.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gxarsevpp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/gdmzvwajt.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gwqfltdce.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/geoumtwop.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/ggmjvjeay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gjeiqaold.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gtqmksmdl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gmuoxscek.sHtML

[Q22] 排序
来源：http://m.share.epnwcf.com/Article/details/gbmzefbuq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gupirugbg.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gpcxbiirg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/gzqppcdbi.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/guqlbuoaw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gytpsngcp.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/gxpuijboh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gzjmuykqy.sHtML

[Q26] 计数
来源：http://read.share.tarul.cn/Article/details/gvfusnzpt.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/grlnnjrzv.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gokgsxiad.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gavuqnfff.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gllpihzfj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gkobdnwuz.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gwkqypiym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gwjtjtbkr.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/glrexhwiu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gmlasoptb.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gbuaqmklc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gmevrunyb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gbtnjqpqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gbgwcvqav.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gnlnrezun.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/gzsligtwu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gzpbosjsr.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/guuwjqkuu.sHtML

SELECT * FROM (
来源：http://www.blog.epnwcf.com/Article/details/gogmdxibn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/guzevdopi.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxzemedh.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gyzdclytx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gvnhvjpdx.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gerwfmhpu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gmlzsfquw.sHtML

[Q37] 右连接
来源：http://www.share.tarul.cn/Article/details/gzajgbmdu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gpryjivwp.sHtML


<!-- 参考信息 -->