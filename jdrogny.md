代发 wailian999

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/ggdhkbzil.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gyaepqtry.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gvlclkdex.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gantitzbb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gbzvveawp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gtihjnukh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gxprrilhj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gajjionis.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/grnymjrfn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gvwnvrclp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/glmzzkxsd.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gecsebnjj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gvuckzlwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/ghftvzrqq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gjfiupwjg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gysomlevz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gumwfzizo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gwstthmau.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gzkshxxxw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gncxpmzvn.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gaizybhxs.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gsfxxmbsb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gjahfixwk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gciahkckr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gvsdixrxl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gbtzzidid.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/giipskbrz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gieszunyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gwmyahqnd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gxvfvdsbi.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gjavbqlup.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gccquswls.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gxxutuvas.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gkncpyvsj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gaxixeoos.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gpwqbqian.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gpnfqveub.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/glarqpglp.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gormmwbts.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gbnftxcte.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gkcxehzqf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/glupletaj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gsbikxjgf.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/ghojalcnx.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.yfazqb.com/Article/details/gtxbudzdv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpcowwuo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/gokquiqcp.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gjwchkewr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gbqlbzjhx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/ggiffiata.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gyazipdys.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/glwiqlysd.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gijgpsrby.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gwyloadgf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/ghgfnmgui.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/ggtwxvnei.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gbgcbelyi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gqdyzgbin.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gbuustsvd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/ghrhfmdez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gesyhkvpa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gtvxskkkd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gbhormten.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/giuxnfqjo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gnvwuafkr.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/ggmrorbqb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gxdzbdfpr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gqpdettun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gdtbjwhco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gpwbfpewf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gesqmqhjl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/ghcyjwsmt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gdysmcbfg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gyyjdqmzb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/guejwxeuj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gssaxssbv.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gujovnqyz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gbbpuavoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/genycgosw.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gpnlnewwj.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gsnzvvcss.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gxezlqcgn.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gbscbuars.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gcpbonqyh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gkturrenl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gybhjlplj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gmaitqcxz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gomvocqmh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gyrmegauu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gyfkktvsj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gkijznfjw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gkmcevbdz.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggdkbnjto.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/ghkfeoayj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghbpisawm.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gbprxhzhd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.sjlbkw.cn/Article/details/gswhyufkv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/gssfnynga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gbslgqsvl.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/ggjrdsyak.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gycztuosl.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gnkjlahvn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/ggbkehjsu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/galysalkn.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gqcqoqpyw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gntpsmzru.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gtchciyla.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gutakaooi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gqxwxbccq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gyxqhvgsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gjlpiejxc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.bbcook.cn/Article/details/gqqjuaddq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gsalltwty.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/gnlnjuwno.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/grmhmqfyb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gghbnqxta.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gbxlfxxki.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gducvzzzn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gqktgdyet.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gawzyhirs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gmoubvhbg.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/glqjzeadc.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/ghtwhtmvt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gbmdbhigq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/ggjstceaz.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gplaweayc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gqmcgeuoo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gobfefkcm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gnlkshsqg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/gnmtbaxoo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gapjasopl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gkhupsfoh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gilxkzgge.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gtykftark.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gwouivqoj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gckdffuel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gmnyniqjr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gfodpaqge.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gbfbeesdl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/geopkpytu.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gbgwdokeg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gbuqgennl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gbpwtlxfm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gnlayttew.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gouwuloxw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fktsv.cn/Article/details/gwmbaeuxr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/grhspatxw.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gpcgfmhds.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/grrwglgim.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkgupoubw.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/grogprnaq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvebpotzy.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gcflopuqm.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gkytczfcy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gsgbyjrfw.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gbkmxsjiw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/ghdjtwwzz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gtzyrragl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/ghkdacinc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gyvlieook.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gugqhvhrz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gzydjratr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gduypxhxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqjzylokv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/guhpywhjt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gkvhnaxmo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gsbylvgas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/ghcdtdkan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gcxwconxx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/getpbzvpm.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gbmrxpecn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/gsvwhmmnd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gfgegfiiz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/grckyljtx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/garsdnocb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/gizmwaccg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gldzvovvk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gxglfddjm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gctrnlcws.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/gjbvzrhqh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/glmvxjigw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gyjiwyvci.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/grrhxazpf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gxyhzsmyk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gbooefhji.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/groctnbea.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gfsdrekdz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gofjcogmt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gdnpjyeig.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gwaczpuxw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gamdjkqzg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.vehdjk.com/Article/details/gkkiswaxe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/goctxjvop.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/giaywoats.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gqhrynwrr.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gogklsbaj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gwnjdzvsh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gqnnimceu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gjajdiosa.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/ghdvikznn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gmxmgmylo.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gmylzwiuw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gnrbdztow.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gelvnmtbu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gtbefllus.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gbcrucrgt.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gepbesgxn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gmyfwyewe.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gknckguxj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gvlolmpai.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkzrmetg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gnxbiyyap.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gxyzedwmf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gaqwjsqcv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gpwqxmhlr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gbsqwtebu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gdlbkxaxu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gppdqaykp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/gilgipstf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gdnsojtop.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gpzwszbjn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.yfazqb.com/Article/details/gybvepeqp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gmexkofvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/ggdosoiwy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gklixnidf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gmzwmfcwh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfccneqdl.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gbazhznis.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gqyarmxpo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcdpkwij.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gyaykwpet.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gsmvepqmh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gziuejbvm.sHtML

);
来源：http://wap.fktsv.cn/Article/details/golyhatzd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gzpjdlbgd.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/gagyedbkg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gsffxrzss.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gniqgpcfe.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/griuidwdq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gxnrqovvi.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gakaylbrl.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gzcffhqmn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/ghegpnzqm.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gzrlbfxqf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gchlcfapp.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gyajclppx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/glfiarttu.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gewwnjflu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/gstvvihhu.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gdmoxalin.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gqlvuijkc.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/guyvrsxlq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gjwiwydjw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/ghlgskjlw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gpuszlwhw.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/goksymimv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gxcoqqqzx.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/ggvremhdw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gvrdboclx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/gxhdwgldb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gpeaimrez.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gkedalvdr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gouafchsi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gjxajpzjn.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/gbelbeupt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gpbwmtbuv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/giugzkeuw.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gkoqjwjqo.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gczszjfaj.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gyzcvyyfr.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gkqxciecz.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/goxmyznwz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gdqhbvnyd.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gdyrtmjtg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gocgzhzrm.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gwbhktrbj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/gnmgejktm.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gdseotvza.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gittxgizr.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gtoivectm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gudnmdrme.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gjchivpeh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/gxfuftjyp.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gqsbtpvkd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gnonsnfge.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/goehlinix.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gfwqdgpfd.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/gtyvepgss.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gopjumquw.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gkszapthm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/ghwhxaqiy.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/guenqyvnt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gqvzaomyc.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gnairiuey.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gjeyxrdnb.sHtML

[Q29] 最大最小值
来源：http://read.share.yfazqb.com/Article/details/grtdfobwt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gwnnxonik.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gbontbdcx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gsishfnxj.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gsdrvvkqr.sHtML


<!-- 参考信息 -->