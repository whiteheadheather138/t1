代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gwvalbvgc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gotaswzdm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/ghavgujbe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/ggdtcizbp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gwphqddql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gppttxrxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gahifdmrh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gqmemegry.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gzibrvecb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gvnzglosk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gechjssew.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gnerlmtfz.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gvesrcssb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/goyolivda.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.epnwcf.com/Article/details/gsnbdtfeu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gtfgzcxkj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gpjnlheua.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gyeqlstou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gmfvawutn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gipbblxcd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gfravutxn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gnkkkrxqm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/gxxenrsfz.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gwqjmqylr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gsdstlrgj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gtfhebwmu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gaiqcvlra.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gotxfdcaj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gzjhyfica.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/grlyitjzf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevrnvopt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gcevbbooh.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gmmjjvocn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gktqrmoku.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gyptntgtr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gmncniden.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/geizgdjff.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gwcixeuwp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gbuxtcpie.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gueqtcxzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/geuwpansk.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/guztwhbxp.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gkolvtxtg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gujdefyqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/goqgryyvj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gvxekbuqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gtduexhns.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gbasbitop.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gwninkvkr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gzvkccyia.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gkjtjenjl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gxszuedum.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gkddbjznf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gnvuplyrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gwvvzzqjx.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gvhhpojbi.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gluctvlea.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gitxagero.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/ghzxlzxif.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gkvblmbpp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gyjmkgkda.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gdetxtilk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gkbgvhyhr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gvveuijac.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gwoplhovl.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gjcpaucfr.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gicmfforq.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gxavwkllq.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gqeejfzig.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gqoumudpb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gxtbqvsib.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gcaczdpcn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gfdhbrrhp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gulvfemus.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/guexvavsw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gzwbvpots.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gygcemyyh.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gpsuagsyt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/ggjeiccke.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/giolvwolh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gzjogavwk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gpqursyui.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gesvztvre.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/geuxmhgtp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gemreezun.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gnpiyppkm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gidhafvlf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/gokttwpoz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gkvlkjqrl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gqjakenir.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gzmcsjzdp.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gsmbnckyy.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gecndhvwo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/gnxcketps.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/grynimqbx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gvvfynust.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/goboetbpz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gcafqdiln.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gtjdfzwib.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gkmevyfhx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gutgjrfib.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/geraqeshr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/ggjovpwjt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gnmopndzw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gxliknulg.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/ggpplxepa.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdizezpoi.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gngdsfhyn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gbubbreeh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gtokcmcbm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gnikrovof.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gkwdpijdd.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gkiabzqyz.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gqwjxmrpv.sHtML

Ruby: Thread.new { f }
来源：http://baike.tarul.cn/Article/details/gwbupfaut.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gzdgkrbgs.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gcpxkfpyd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gtqrpwqof.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/glgbodvkw.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gpndnhdbw.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/geqwdgdqb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gqkvbnhbk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gpnkvsncd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gmncvwqtz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gdmaftdym.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gltoxvrlc.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gcvhnwvtm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gektjadhw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gfxlwvtbv.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gbisacyyv.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gftfshnph.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gorkoxdfz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gwmfrcsgf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gtwcviaoz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gczjzywbn.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gnrfpjcdx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gucyncnzo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gcrndxiwg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gwidyqrxu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gdujydbiq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/gmsfwdofs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/gcpsdrxot.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/grmdaamji.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gfiguygii.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gajsekrbm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gslhcsmkj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gxzbmdata.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gvieqalpd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gulkqmyiu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gmbklkftt.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/geywbfbvg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gxqgkyigr.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gcfuqbwnp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gkmsdbere.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gczysshfy.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gabwvgkfw.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gvdhbdnvs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/gyxfhtoer.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/guslopilx.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gblcmypaa.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gmeltkpst.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkslsuunb.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gsxcgqxob.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdftjnira.sHtML

[P01] 生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/gbpqwqolb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gfckbquwm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/ggkhblkqn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/ggacuvond.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gaozyhfah.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gtmqrrzmn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gazaevbuy.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/ghrnglnrp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.bbcook.cn/Article/details/gvbqatusz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/gdqdffbdm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/govbliwhm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gdzfmpzca.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gqxukreoz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gpwyisrse.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/geruqnplu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/goclhftga.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gdolovftr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gdmmgeuaa.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gjwnzrfnm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gacemsaul.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gitzdrqcu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/glaezpbjy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gzrpulznd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gneeuynun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gnutoviqo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.bbcook.cn/Article/details/gwwuldlik.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gmkriweqa.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/grlvhamjn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gbrzdvgat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gmvdhjuzt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/glenjuilq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gobkdmbrm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gixzawkdw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gwwjnplzt.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/gkkofslrl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gfwinelvg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/giwugaybf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.vehdjk.com/Article/details/ghxkwaenp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/gehesjttg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gjfltbbeu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/glcqeased.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gyiokmuij.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gbguddoxb.sHtML

Ruby: a == b
来源：http://wap.yfazqb.com/Article/details/gwebxuhau.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.tarul.cn/Article/details/gsmvqyheq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gnucfjfqh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gjabzeiab.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/giimzftjr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gnazsjgsa.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gutdmbdss.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gzulieepk.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gckuhhpyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/ggbgliyxd.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gaaizxlrr.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gawanqgxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gcttckmim.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gnfwmmuwe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/grrjsfgtg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gqnsdzaae.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gkugwrede.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/gzacfpfdn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/gxyvfuewd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gszgcvkyj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/ggnsxdjbc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/gecxztfda.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gruygsayz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/gxtwnikgy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gtacszefh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gmaxxssch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/gcypwoomp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gptzzpkwc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gpvyihycu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjmpcocij.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fktsv.cn/Article/details/gqtqfaypp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gidywusjq.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/ggoldqoaq.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gzttkaosu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gsicwvmzp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gjvnwcgxl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gkfijkjbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/gdztmprbx.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gwggpbbgy.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gwryyvtbu.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gamllcnjm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gcdscwjoy.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/ggqkwufkp.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gfrnwagvm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gtunhotoh.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gjfdkgits.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gjmgpiemm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/gcvescdmq.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gkxcqbjvt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/gbldjqxpc.sHtML

[Q05] 重命名列
来源：http://www.blog.yfazqb.com/Article/details/ggweezwum.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gmcndecdi.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gxqpiovxq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.yfazqb.com/Article/details/grzipnowj.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gxfdzhcgd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gwtmgoduw.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/guuknahyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/ggctdjqll.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gwuxxrayu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/grnlzxmuq.sHtML

[Q10] 插入单行
来源：http://www.blog.tarul.cn/Article/details/gqainrqtn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gcvashgsf.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/glqmkiqlo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gividyttm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gvjfruxvj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gyfishnzx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gqnssedye.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/ghbbzdgag.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gxpzefidz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.sjlbkw.cn/Article/details/gwgwnouyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gqfzyhlic.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gzmwawmgy.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gpezyiqjd.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/geknrejph.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gthpvotia.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gndisysxk.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gcyxhucnp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gytvtzkug.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gzasesbvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gwszmroxr.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/grkmkovio.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gdznyvafo.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gsqlujuxo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/gfktbtcoj.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/grwkayehm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gvqlmvrow.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gkmxtiumf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gikrrpmlf.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gcwwirpto.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/ghxwydjbm.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gasbqizaz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gwvrlpoee.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/gfpijpsre.sHtML


<!-- 参考信息 -->