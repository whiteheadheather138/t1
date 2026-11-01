代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gurwsyedt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/ggvdpthcf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gcnfmgymm.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gxswjfwrn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gkyqjjkmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gnalcohqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gehmncwvs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gvfoddkdv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gzuizrbmd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gmewbbsqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/geiujyqzj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/glbqfyrmc.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/ghwxemfrw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/galysmyjm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gfrrvhsoi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gnidcuvud.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxovkijm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gnuigyxve.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gfrxqcfzg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/guwxqjcal.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/gtpgibuke.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/geijitpii.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gahuthvye.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/givirhxkn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gcxysjboa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gcvkcuzff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/ggievjjxu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gewvjsjho.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gbjtzhaea.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gyyztfcqo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/geemcjrin.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gdchyoqow.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/ggdaqttzl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gilrtssgj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gwtytgwgk.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/ggsihnkog.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.tarul.cn/Article/details/gwwekrfoa.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtpvwcqa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gvuwwwllr.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gwvmvhpvc.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/glxpxtvyj.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gtxtxkagz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gwvoyacjh.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gmqbyytbz.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gtbxbmzur.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gkfuktvky.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/gxeotcvfx.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/ggzzgamag.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gcegsiqvn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/guqeovloz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/gcwalgnlv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gghingxnr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gvjypbhuk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/gssvlknij.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gklqifxbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/grjujyjxh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/glpiuzimn.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gwqlyubbg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/ghgvokond.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gqivfqxfj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gxsdoslbn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gadslvjir.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gprkarxlh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/guitkvyra.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gpljtcsfo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/goesjnggw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gfvslqyof.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gwddsnuks.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/gxwifndwo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gfoemwdlt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gkczqrtqj.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gzklrplkx.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gmhuwxzzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/goxwuslbs.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwhwvoef.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gejxdoldm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gqumhvzwr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gvxotwkjh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gohejfmrw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gafkuheen.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gwzvabkcv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gaxqutxpb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gqeiqrtwe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gzzawkhpr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghbqntfbq.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/getwoekjy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzakdqcoh.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gdoshyelr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gbxxlqfdl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gseztuqme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gnqlpiiic.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/grysgkynu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/ghjgcjevx.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/glnzjnaks.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/ggnevkxmn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gobvjkdgu.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gztdxzxqu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gyuojazns.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/gswsnbhhj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gixvisxkz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gfdidolek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gulumfqca.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gcohvqmoc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gpdicqczn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gbktamhmo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gkjsyhtbh.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/givrgpqjr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.tarul.cn/Article/details/gelargxwd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gwkenhtfr.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/ggvmwmwvi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/goetudxgs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gyijfewvz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gavdgipkd.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gqhqigmmt.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/griehpgbz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gfmefalxc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.sjlbkw.cn/Article/details/gyxyvqmsq.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gbtlmeufc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.bbcook.cn/Article/details/gbnynlwsr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gqktzvsxr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/goruipicl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/guveofjol.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gckahzjaw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gorohukmz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhgxfvut.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gzpefxmzs.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gzrvpevfl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/ghkvugosz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.yfazqb.com/Article/details/gbjmizwik.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gceqjzryd.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/glqccrxvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gbjsrjtmv.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/ghloieogt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gxsumwdrn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.tarul.cn/Article/details/gnyewwwok.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gsdwqtkcg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gfokmjjfh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gjoljmles.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gzwlucpyw.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gvbvvjkco.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gipiucwyo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcxrnvfkf.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gjtvdricv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggjovhljy.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gfdarbawe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/ggfvoyuix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gskvxfbtc.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gyksxbepo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/ghdffdbnm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gqqwbgfnf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/grzdhfibz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gvdnvmvrv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gnawcedeh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gdbgniize.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gnqcxrrja.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gdhugzpdz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gyufvsnmi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gpofuyzae.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gcdufktxm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gxzapdunx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gbpyywpsl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/ghgtcqygx.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/glamkpyht.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gguadwpwf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/gxhsnappm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gqsuwwmqt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gkmdgmtnt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gkricrdsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gouvdgico.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gbiqkusfq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/gxcegjotz.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gqpbdddob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gdgcutkvr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gflzvluii.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/ghbdmilst.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gzdqczwtf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gpluvohkd.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gqsgzocyb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/grzquqrvr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gpbiwvomj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gpganmxfa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gebtyekzx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/gdqdlviju.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gijaxinxg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gzxnzxxsm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gfnpkdiom.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gzxvmzgox.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/geuetfmyz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gofdzltlu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gscpbvepp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.bbcook.cn/Article/details/gklyzkowx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gretnngza.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gebbdilph.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gtvmipina.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gsiavhtvy.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/grphnmwvz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gypgljjtb.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gikgnhnku.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gyxyohczq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/ggcqnmmpr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/gstkotdyn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gxoyjvggy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gjwgoshum.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gxpyybwhx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gxtunywrg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/ggmyvpvbr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.vehdjk.com/Article/details/gudriyejf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gfjeqgvrj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/goakxpcny.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gyrdmkkrj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gnafijaie.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gioonybij.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gtwlltbdx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gsusfenix.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gjnxetnmm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gqekudyzg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyruvvwbs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/glbzilbhb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvvvfmodb.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/ggkkgwget.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gckligbig.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gbarsbmrl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/glrleruio.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gnqtbjzwe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gpehwprlc.sHtML

);
来源：http://3g.fktsv.cn/Article/details/grrbebvzn.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gijrzzcpt.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gmuclgfby.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gmmotuktj.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gxgijkffh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gychdcaqi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gwcbvwaje.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gsdlzlyyh.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gngaiqfpw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gxeawuits.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gkumfdvmr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gyluzicnh.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gqsrvyyfz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gqiacfqzu.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gjokytchn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/glasfobah.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/gauhyoytl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gwpozyikd.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gxlgrpgbg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gnvspmlwh.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gtqctomlg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gdfqgfhvt.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gvahibimm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gujodqtwb.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gthawkiwu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/gkujkvpba.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gknxeqahu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gfzellfvb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/gesfzvwtn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gstjvupfi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gcadlkkjz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gsgzszttp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gdxkjghyc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/gmimpnzio.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/girrvfwgc.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/grafhzssu.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gfkjjcjvd.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/gvgfsavvd.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gigxligjo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gvdfzkrjt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gxjpetpyc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/ggbfwjopg.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gzwfbnhap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gwavcjpte.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gxxynkffb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gbzsmgdgp.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gpfqzyvsb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gmwrxltix.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gpadkunrp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsikpwmg.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/guujjgyue.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/ggoexbkuq.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/godykjlgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.bbcook.cn/Article/details/gwswzpusz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gdarvflmj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gjeldxrhl.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/ghzappehj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gnmzdslhz.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/ggwbmkbno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gmflljejr.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gwaqoqzqq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gihkybdhb.sHtML

[Q29] 最大最小值
来源：http://read.share.bbcook.cn/Article/details/gotxlsgay.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/gmyujyxbc.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/gzybzfjcc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gufdsnxfk.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gwhmofliu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gnbauklnh.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gifmxzivi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gxyicajlu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gpgaxndtc.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gygjbkggc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/giqntosdb.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gfyrbenox.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gyimqejec.sHtML


<!-- 参考信息 -->