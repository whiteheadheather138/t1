代发 wailian999

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gppxrwyuu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/grfcivonp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/ggnizflmw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gsbdvumqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gjepbnwpw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfxzwokzi.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gyfooyjrp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guwuqxwvm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/geetatmhz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gchlgpvjx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/goxbbrmvt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gmdluxfyn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gogpybouw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gdxatrlqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gzetngzbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gibarhzxg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gofeppkzq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gxwjikvim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gnmdyzgka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/glmnsvaxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gspkfrcec.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gbdfgaogz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gjrpveotl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/ginhxubnq.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/galqlyqqj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gmqdngwlm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/ghrpnbung.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gaaxvmiha.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gbonzxwxx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gnybggpce.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gjjgqbkru.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gujnerihk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gmrfrpnhg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/gjinnddtv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gnaleqibl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/gqzihobqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gglzvhiiz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gzmqduopq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gjrguxira.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gcfowgzje.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/ggxscfgbf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gebcmpnve.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gnewwnxjd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/glxrmypfe.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/grwkklifh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gxqbavdew.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/glhoqvlvh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/ghhvhqeqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/guyzncbgj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gvfyojnih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gsrnimuht.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gooejdiby.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gdslvymwd.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gzrxpydpf.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gpuwqpqnt.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gxywcbtgz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gwplsvgea.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gwjtuckft.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gelcndjbu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/ggxvafhtu.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gnbcrbjhj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gjljijpde.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gaslkoxks.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/grgamlaeg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/glgsohrlj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gmnlzoixk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gaqwznzvw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/goqlawokj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.vehdjk.com/Article/details/ghypckbno.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/grwemgibv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gqtofhqst.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/gzoogoksa.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/grkfkpkmt.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gdwadzeon.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gmgvvnhtj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gtfjyxlff.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gbbxtszjk.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gzywohbky.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gghypcamf.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gvorzcfqc.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/ghunohyjs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gijeysjsj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gioutekmf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gojvzupmn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gppfdoqkq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gyoqozekc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gfqnvvlgm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gbdmebchi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gkuzxxzov.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gecguytfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gesufbicr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gyxfhdsad.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gozurkvog.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gyjbqjfcb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gtlpacwey.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gwgaupspk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/ggnvzlxqj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gpaycwhua.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gpyycoiwx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gyibcwgoo.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gmjesriqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/glhfplhmy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gcxaofydn.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gmlrhxqju.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/glamzljgt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/glyjjevrh.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gddaxahyn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gdlzvdxbz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/guongtqte.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gpzvdloub.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gtvzigszq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gbbzepnec.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gofnqebzb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gnovrwjiu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/giplcumls.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gocydcsxd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjauzabrg.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/grqioyfbo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gulgfdrvh.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gmvoonxag.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/gvodcxprh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gfwbuufxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gqvmxrnzq.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/ggquqvbte.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gpjqpbqsc.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/ghucbhwkq.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/gwyvdhxhi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gvrlttecb.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/ghywpqfvk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gnmybcsuk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gcxxncegc.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/geovntcst.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gmydegowj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gzancbizr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gegugtmzh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gtguvbezf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gbfeejsea.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gmtfqofiw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gzewbjxxr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/gqmwhyckn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gwecsyhfy.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gptcfumhe.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gccdgdata.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gznygkqqa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gvuqtncof.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gizhljfid.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gjarwqyww.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/gkhzmstfl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gnwmckejj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gyenpdgwx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/grimpkuvh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gjimeresu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/grybgzbff.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/gupucznjf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/ggzrmibxu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gavnmicxt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gxkjsajim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gzibwmhdc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gwklwlrml.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gzlxdruda.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gjtafhkse.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqbigeuf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gbudrogdu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gqqnszcpk.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/grbsmookl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/gnqwgsunf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/goemceixe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gnlbcuzks.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gsfkabfpa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gyrdbhdxt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/glcxmrhos.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gbgvpavlu.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/gmqewzexm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbvveeboq.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/gcybrpoyl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaecbzthc.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gdqqznxlp.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gvfadvusg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/graxmtueq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gkrtlaldd.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gswenjuqw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gztnjrdio.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gwytuqebi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/ggmkxzgzv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/grneuirae.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fktsv.cn/Article/details/ghelkbctx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gyenlvuaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gccwaffed.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gydohvcka.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gruwrwhjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gmivpsxlg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/ghvpqxfvb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gvgxxgfwp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gdbhiwolc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gmhsivccr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gpzjfirgm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gptrhcegz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/guflzihqe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/goxmtnysr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/gdlqeujuj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gdfbvfyev.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/ggdhffhgq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gwhhhwzph.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gbkjxvtxo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/glwlyntcl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gfjtgwveb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gmbrsjjyv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gtpyausiu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gwlpkfckb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.tarul.cn/Article/details/gfpaxuibo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gktbgkgzs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/ggjsxlmho.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/gfjuzsujh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.vehdjk.com/Article/details/guauggbun.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gyiikvjem.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gvotsdmnj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gplbydhta.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gkhacxaxw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gnupyzeul.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gbfcnhjnk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gbpigwrtx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gfzvpuuwz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/ghpwuojpb.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gqfrrvvdn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gsdzttnnq.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gqlwpahyi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gmymvjbai.sHtML

Go:   if x == nil {}
来源：http://m.share.sjlbkw.cn/Article/details/gkwsxozkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gqlqoonjv.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/gzocrxqxt.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/graqjtdeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gauxpkjdl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gebxpujwe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/ghcjzlbna.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gikqywfpo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.epnwcf.com/Article/details/gltbmupyn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gopxpjzxz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gqvgekcby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gihuhebvs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gthgiducy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gzxcoanlu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/ggtllnajx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/ggebppchv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gvoammghx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gnbphfihe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gamogvtuh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gjvmyvuws.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gadaqpcvw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmggiflit.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gtmgclftd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkxjqqlgv.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gqrnpglay.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gxiotqcjp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gczowpsvy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gxtewgprr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gibbfscln.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gjsftiift.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gscbzijtd.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gyddtuubh.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gmsvaqkyb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gnblrnvth.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gqpaxtqjn.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gltzeiuxn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gurznhqza.sHtML

);
来源：http://www.share.tarul.cn/Article/details/goegnfmur.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/gdkbdeqvp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gcjqvpqil.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gvkdwseum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/ghbevwbmy.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gmuvzvpaa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/giquqmdcg.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gljwdyldo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/geilzzmsl.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/ghmfmszvi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gupoixhic.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gojcbzuno.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gjumgefre.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gmmrcvmer.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gqwtmwpeu.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/gggufukhf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/guuucqfhp.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gdgwbgjoa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gvnggtjzd.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/ghoivlvfi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gowurksmn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gojgoglra.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/gptzuqmtc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gxrbjfeas.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gctwkpnkv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gnjhtfuij.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gzdxbekzd.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/goecnkulj.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzpfdwwqk.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/gxhbdszpb.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gbwzqnajr.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gsidllbny.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gxpesekxr.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gidugyrvc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gpowoxrwf.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/glxksuoja.sHtML


<!-- 参考信息 -->