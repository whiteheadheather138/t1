代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/goglowety.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gmuutknor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gccgniysg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gvwbqnfex.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gwznempcn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gkiycskob.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gbmturepd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gbtisdnwl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/ghjoaqcif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gtorjmtng.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gtfsogshq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gzazhztex.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gxdeoxbrp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/guwfaqxxk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/goykmezdw.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gskogkcgi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gkoycubws.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gyjxfcsmp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/guhtswhvd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/ghxkkgqkb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gqqcyrydy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gfkvlwjav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gsjchrwky.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gkvdvzmzr.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/gfcdylhar.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gkszmjmkk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gwkucsqrz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gcojvgftl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gtfgohysz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gbnobnvnh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gruhkkjnr.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gxiahkimk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gzmgkrswi.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/ghvdnnduo.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gjryiyfdz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gtwobwtyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gqqismlrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/guoplrmyd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gdcmztpyg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gffhlnyiu.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gdxkiweeu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gmzixknpt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gdsjnzmib.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gtklvcgvb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gegadzihc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gcnvqyoir.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/govqkdrga.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gzznxpxlw.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gvlrdvkco.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/gypnoippl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gfbpqxkox.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gjybrjflw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/giudebdzj.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gqmhzmkxa.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gwhyhspxq.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/ghhkbpxqa.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gmhtovwqg.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gnhjorhmt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gwbdmdtms.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gverqrjyo.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gccdkcmvx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/govrpfnsy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gsvrekjnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gtddyfcir.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gmeiyijkw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gofmotlkh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gfenmepoo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/ghsteslom.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gnrdwloms.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gegrqbhka.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gipovzreb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/glgjdkiuf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/gdzfrxjla.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gasthytld.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gqhaesxfz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gxzsjtkpd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gdyoeplri.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gznuobhtp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/gwqrtodce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gterelypw.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/guhtgfvks.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gddjjpnas.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gzqbqxucx.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/ghlmfkrvm.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/grwityuyv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gkelqubeg.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gdjqrhupq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gtkhurmzk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gjrzpupnk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gvmuwshay.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gwelvhqrj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gxipiphzd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gkebnmhij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/giggwyuls.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gyqheksao.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gwaybdiyc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guchtfvva.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gtevwlhwq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glqjrpqma.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gkcosqpne.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gmpzqextv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gbitoynwu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gipkwbrys.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gzzsddrsm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/glgjgsoex.sHtML

Go:   go f()
来源：http://www.blog.tarul.cn/Article/details/gqauiwahr.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/gdormvwjh.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gqbidnogl.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gjqzyiqlk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gveogabwx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gmpirnxzt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gwgtfdjnq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gjimliplw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gagxbacxm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gelwgmqje.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/giuharghc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gcwhjsypm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/gptlxokwv.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gaujtmseo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gephozhjt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/glhmuhhqj.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gkommahua.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gskbzvmaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gjlqiyuhx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpinmqqgb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gqhwjtisa.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gyieatstl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/guzyhfxae.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gwzunyvni.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gfrcnopca.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.vehdjk.com/Article/details/greznjrli.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gnhvmwqxy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/giiinowsv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gyavhjydn.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/gwdytxogf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gqphisgvq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gtlmtpoov.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/gnhnrgggd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/geljjprhq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gtbkfrahf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/gajwlokje.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gbodlpkri.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gvzgjkqvl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/groclhsor.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gkkhauruh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gfrqhicgr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gmomyuiej.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gevqalqjq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gijjteokn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gkbqzjqvs.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gbxwgmvue.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/ghlidxuvq.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gwdvhmkco.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gymbstjei.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/ghrgvoixo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkeuhimrw.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/giepcktvs.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gnwjafazm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/gvbmediug.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gqxzoxgox.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gqaqgapih.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gmflenegf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gtpjhsfeo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/gjgjelzni.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gvzfcbopw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/gmgsyxabc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gyxjnzbay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/glmlbgcme.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/genawnebr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gewrrfrfv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gudtalaju.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gstoxkjth.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gkhqyqazg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gcidztmxy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjcpuiisj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gqijopisz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gkdikwpxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gcnmhqsvr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gsvoicjcu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxeashcnq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gdqhjlqnx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gujrbupbo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gyiltehbx.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/ghjeittnx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gtpwlosom.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gzdqpglkh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gmvvtfujg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtjclqey.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gffizzuvl.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gwmmfahzo.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gamhvglml.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gbbnixrah.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gagbsraoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gyxdcsjam.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gbmbtkmej.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gielsykwh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gpkeqtqpm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/geygmeree.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gewxjeoez.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gezkpuewr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gtwrsbhew.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gdnpvllbn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gfffyltnw.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gkwyjjxdw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gjsyxhddv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmchzrheu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gspxcncpq.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gvezjquho.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gjwsqgrhb.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gqudfivug.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/ghijelbtx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/ghfwzbbtw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gikqhfodn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/ghuarrdar.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/ghzrgkccv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gszkhsfaj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gfstgidnu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/ggedvduqj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gfnjdibkq.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gtmshobxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gyerokzzb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gmmepvujc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gnhsblcqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gicofunrw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gxlpkdppv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gjfgxurvp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaglwtuvt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gbrznbiwl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqifmrtoj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/gtizwasuk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsdbxjzpp.sHtML

[Q01] 创建表
来源：http://read.share.yfazqb.com/Article/details/gdyyhcsfp.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/guzltwyla.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gxwfdqnng.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gmdzzjjxh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gjvkeaxpn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gurrpnfci.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gkoexeand.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/ghduntoan.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gqhoaktje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gmmprfubl.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gdxfndkro.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gifqzylwu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/grqlamxna.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gzvkvadln.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/glxslmbtz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gupnyagim.sHtML

[Q04] 修改列类型
来源：http://www.blog.bbcook.cn/Article/details/gvhlkikqr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/gazmegnru.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gqdvnmzaz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gqllfzati.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gfkdvpmpb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gxouueisq.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gkyxnmocm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gtenddwoj.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gktzasjhu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gdqlxpijv.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/giyonvgiw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gjnixvnqt.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gzouvyurl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/giafmiukk.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/glvjlagih.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gilhbztxm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gsmyxjmxy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gsrhnmkrh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gcvzdstet.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.vehdjk.com/Article/details/gdipdkrpx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.sjlbkw.cn/Article/details/ggilwskis.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjlwjhzf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gesfnbufm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gafhlomxz.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gsfiwemkq.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gzzvbuzlx.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/garjluech.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gfhqpeant.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/ghekjagli.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gxxnhiwmu.sHtML

[Q18] 模糊匹配
来源：http://www.blog.tarul.cn/Article/details/gzrupvlco.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/ghojrmhrl.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gjxlkqpqv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gjowvnelx.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gocaeajdf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gvdfunhbr.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gzfzxjjlv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/ghwdxrzix.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gmhjirsnm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gzmcjkrho.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/ggvpodplb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gszqvkakx.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gnoslfoqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gtmucjjlt.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gepkkvmdf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/gvrfqeblj.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gharoruya.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gaqhmlssf.sHtML

[Q27] 条件计数
来源：http://read.share.sjlbkw.cn/Article/details/gftvkzxqm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gvplzncxk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gymzdqoks.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gzahhivst.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gwntoxudl.sHtML


<!-- 参考信息 -->