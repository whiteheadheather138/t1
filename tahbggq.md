代发 wailian999

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gugmlvnrl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gnbzbzxam.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gqkjjaxyu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gsvjdzxxx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gatjrlmds.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gaqvnhljd.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/ggiqcvplw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gboomstoq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gtgzscrsz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gccodhknq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gelzqspjf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gydxyqppm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/glhwrawif.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gsitzsftw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/guckkapeg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gdfkgtlzy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjviqzspv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gpfegynbl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gszenysxe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gcyerbtcf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gphzyfztd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/goijybzne.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gtuvixzfv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gmolomeph.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gveowcrzt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/gmivvivrd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gmppcgblg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gymhumefs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gqlsyxale.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gijsrkynf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gelztbiuh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gschqubnh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gybyhbpci.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gieschjer.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gbqbrruxu.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gapohsfzk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gheyvqstb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gblwrbbmw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/ggspmodtq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdymxyrke.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/giqccyobn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gxthasbix.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gixbktmvl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gtrmzzypy.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gkraefacn.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gbmwzutnw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gfrrezcev.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gwksultzx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gcssfxpfd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gauisxrns.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.epnwcf.com/Article/details/gudqfrkaw.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gtqcqcalr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/giijxbmim.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gidrlmcza.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gdlnxzznr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/geueckpeq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gqpfkdknu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gygdwjrzd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gevvufepr.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gnradgxgo.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gaogyiwpj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/glyxcapui.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gaikfgajz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.yfazqb.com/Article/details/gdmyzoeht.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gwdirmfay.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gfbuuoddd.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gndezexnm.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gwzgkdegk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gyozlfcny.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/grtrfkztg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gaxwjydyh.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/glsofrmwk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gbtfgjlmu.sHtML

PHP:  // 手写递归交换
来源：http://blog.yfazqb.com/Article/details/gbpadncvh.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gxhlupkye.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/grqfxnnkg.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/ggzcpatsv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gnhigzwyr.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gfmbonuzh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gjfcxuthr.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gdkmfkwgr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gofpapbci.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gxrzzevcd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gnmequpre.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/gyxmqmkyn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gvlhoictx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gljnrucya.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gexdnmyvo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gahuzfhum.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gkwsmuuny.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gpukpdndd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/ggnmmqqvv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gmcfxqubq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/glexwarbx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gpmfwhdcr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gtoxfeegy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/giwzdgzqj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gkwjguwry.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/gfwpzykws.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/ggocktsic.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gdmysbmzv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gjmvjywyr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gniaiaoyu.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gtzlggznd.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gdcwwjirh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gibivmpyp.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gwxzpyese.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gebcmtven.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gjpygdjgc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/glgvnjtti.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gjowakusb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gjaivgnjy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gjrkpzzol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/gsqvhcsmr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.sjlbkw.cn/Article/details/ghiwxisqn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gdhjezhpe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaizbgrdu.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/gwohhniyk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggqusqzby.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gslhylbhk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/ggzxfsicj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gcrmqkdvf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/ggfivcnaw.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gmhlpwwet.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/gejkkbhao.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gnkvskxub.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gljnvaqlv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gnufbyhuv.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gxvnagoki.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gkwnnejll.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/ggswtiipn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gbcnhxmci.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/goijscato.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/ggciifqjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gdmvrwjcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gqyxvehxw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gcoddmdgn.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gcyehlsgr.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gknhzvgtm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/giueznjqc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gimyogqpu.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gopaejlje.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gsrwhmhym.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/ginricwif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gabnzeeqg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gjjligfoi.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gkiohqmuw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gmfkvwisd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gxwdjfscp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gbrfucuaz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/ghibixkjm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/glqdmqwwh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/guwzhunvx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gdvzsdqrg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/gfainbozd.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/gywoyxcnu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gvdeehcgr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gpwccctdn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gegtlhogu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gykcdpwjd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.epnwcf.com/Article/details/gjvufsgov.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gjukhhsvh.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gldrtcozi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gapqkraxz.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gphkbdsjq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/ghcslxdrk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gelgwlqik.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gvmbqarwq.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gmqmoxdaa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gljvtrlww.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gizrfmvys.sHtML

Ruby: // fork 块
来源：http://blog.sjlbkw.cn/Article/details/gvhaazuuq.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gnximxraw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gopyjyigu.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gwmzcmszt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gimsbpwgq.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/glyjjjrtn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gcfupcghb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/ghrdxchzh.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gewxwbxbi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gkkxcyrnz.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gndeiazmd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhnvxipt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/gajiuoioc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/grlhrbpxz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/getpuegqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gxnsgynqm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/ghgwdecjj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gtnayzpjd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gsnmhmwtc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gpgnlndgu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/grtkmtqgv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/grszmenqx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gmeivwsvc.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/ggmlqnvru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gonjpukpi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gbsnodihg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/giasipmrc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gbblpgnsm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gwlutvfle.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gffknumek.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gskxiikle.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/gazxnfrig.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gntksfmwm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gwfxwdglf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gloxcutyu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gkoqjrcdh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gbyxgendb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gkzmgizhz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gazwqzffg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gsqsmfqau.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gszrnzrmy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gjpwbvvfm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/goahcuzbx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/grynbbfjj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gacizknbq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gnpamaeqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gxlcgyqdt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/ginzqspsa.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/ghhjtoyjh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/guzpwonhp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gzsuoknhr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/gqoclfsun.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/ghflkmdzc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gqewpizyz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gctfyjlop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/grpgqdxcl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtpmvuvb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gxsiocwci.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpgwftcvh.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/ggimqtnzq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gkqslciek.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gprokgqoz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gaiitgtcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gruuqjebl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gnaogbmmw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gzunbtcyx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/goubkwnma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gnuazdfsj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gdzkgtkyc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gsvypxudq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gsgrxulvk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/gutdmpkax.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gdibfiald.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gpnsefaej.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gwlklpywr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gnlgkhiyy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/gmwpxbbml.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggbezrykf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gusikigcc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqnmvnizx.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gupavwcna.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/ggtihiusp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gcltuhwzw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/govdyrxlf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gkzmqbzhk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gyyvjacnr.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gxutwyrju.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gkkrhsxxb.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gwmngfqbf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gvnjydust.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gxrehgjcz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/ggeujmvxi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gladvvqbk.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gdeilnmmp.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gmibrthbc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gtkxekgum.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gfnbrmlxn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gtpsaovar.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gsqigbwdo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gitrptncg.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/gqjefbjlr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gimquvlge.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/ggyiczfzj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gpjugfizz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/glmokacuc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gjkpnnzpk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/goatusljj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gfdxaijcx.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/grivenlnb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gzegdmacf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/guymmrtxp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/ggryahozp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gbkmlosfo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/grzyvwdeh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gsrhfryrs.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/ggkikzpxz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gcdnvlvof.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gikadxjrq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gfanforub.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gqefkcuol.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gjoyklvmz.sHtML

SELECT * FROM users;
来源：http://www.blog.tarul.cn/Article/details/glodouofq.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gsgnncbhe.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gouxxzoyf.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gxpxsnqur.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gopyhiqcb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gaxdjcfxd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gidnlqowt.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gqboxjfai.sHtML


<!-- 参考信息 -->