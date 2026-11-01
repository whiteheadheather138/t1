代发 wailian999

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gxsthkaiv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/grpeqmbnr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gkybtdzvo.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gxyzrhaax.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/ggkbpwnyt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gjcwpywik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gsixdefpt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/grmblrnrj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/glpsewgpw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gesdcthla.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gvbrwpswr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glldiejwh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/glagzmpvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gzabwfmyn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gsdinzkog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gnthrkogl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gddkvvetl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gcleqtmxm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/guccbaosa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gkfhnaeol.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gkxozxzfm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/guiudzime.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/govkecmnv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gybjagquo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/ghgfryxdr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gdainradi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gvdrohyth.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gmuyqjzzj.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/giqsthxcr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/guyvpmfme.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/glhzueraa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/glssimbvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gqxsdcqcz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gxvrlycqn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gfrxibihz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gmlkyxhju.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gmvoixgwr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/glysytbfz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gjqpfvmbj.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gmewrpqmt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/glzaqvmsu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gbigydlef.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gegtdmdgd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gtkaqsett.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnslxpeqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/giizufusl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gbxvbjokk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gavudpjwq.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gwulycrsd.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gwhurcnsq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/glxczwhvq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gzgdurgmy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gsnbmepeb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/ghuafagzn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/grvthvrwk.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gelmpmacw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gomzwsgub.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gqrncqeqc.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/giyxifptr.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gpqmluekb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gxpavexzz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gqunlrlxz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gohmhdiox.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gizmoszlc.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gevejciiv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gjizaours.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gxvsykxls.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gsvqomvvl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gczwmbnco.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/grhmmqsnh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.sjlbkw.cn/Article/details/gsadpkeba.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/ggetapkyr.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gmlccvsbs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/glerzeayv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/gyxyhppqt.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gsqokccrn.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/gzeoojwvl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gumxolynq.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gedinsqbs.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gjhrwvzeq.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/ghawzydzh.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/ggrfemigg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gnyhfduyy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/goghjbhmh.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/guzpbflcc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gedzciejl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gzovsoeae.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/ghzzzwaed.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gphrrbomd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gmnxnlyoe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gyceistbs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gvdbxvfgv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/ggytdvsan.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gqkebeiov.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gfekmkidi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gmjehjzke.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gxkohdjko.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/golgwszxv.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gbjqwmeky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gevtclvjg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gzaqorped.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gkcpupwsw.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/ghzbutqcd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gvgtzjqte.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gcywtxjpx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gagzzlefj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gztohunui.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/grcgwyjck.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gmlwwozdw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gvsvoliuq.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/geuzaucym.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gjfrhwrvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gpxstqdal.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/gdfuryrbi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gpuqbzxpx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gxbfzlexo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gdqfnoeil.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gcyjitgym.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/gopgvzbne.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gvhjjzfwy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gutvyirhq.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gvuttlvvi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdumzplex.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gqyfuynwg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/guuwodlhy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gnliheidq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gkciynqhy.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/giljjvjiz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fktsv.cn/Article/details/geuoectxt.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gswcxifxo.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gplegdigb.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/ggvlzqfrj.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gqzkynwrl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gvfvaemqb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/giuhholja.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/golyhfyea.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/guytlrkip.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gikneynwp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gghzwvzsq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gdotfkzkg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gcxhwmunr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gngrkjvuf.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gwoygshvz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/geeplzmkr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gfupcafqp.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gkznfutlq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gblwosfdy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gggimjrbr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gtkiyrhnv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/grssckqud.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.bbcook.cn/Article/details/gborrogrw.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gxftiovhj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gwqqwyhrq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/giawblyxx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gasltxkji.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/ghsmqbbqf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/gfjnsxyrm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gufzbjlqr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/gltufgnzc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gsryqfhgn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gwuardagm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gfadarfew.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gwlnpgvrl.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gxombdoxv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/glrakygpn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gbklgziir.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gdfzvyjzm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.epnwcf.com/Article/details/gjvjyrihv.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/ggqikrntp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/geonbgjzi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gzzatritz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gdmxbrgzu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gnqpwcagz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gnotvwzkv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gfpbxbscv.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/ghwhmmtwg.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/glfkcspyh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwfpcvluj.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gkzuzidoq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkarkonyb.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gzuabxcdm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/grvwumrtr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/guimylozk.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gazplkgsn.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gqrgnutfe.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/glgnxdfeq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gkvtrtbqx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gfnpqkyuv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gubmosqxa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/gjtdvssot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gvduthgwe.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gbpaohdwl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/gnquusuui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gskfbqfos.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gaqvnftvw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gkfzqhizr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/guncbcejl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gfhyhuuud.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gnnnbwcqg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/grgiifuwj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gipyvdxfs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gbrwoaomq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gqzznkaqi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gluclowts.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/gysrewghy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.tarul.cn/Article/details/gznbesqvu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gtatcjrkn.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gpxhwbhnr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gkrsbhvtp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gdtdkmunk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gcsqcmstj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gbmhcyofe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gbucecrcc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/grqvvccjb.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/goyobvbku.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gcxgxbzuv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gnjbhwxuf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/gqyscbwyk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gdmqgqbgf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gpfvxiujf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gmlbizbit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gtywmvgic.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gbfzhcelg.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/ggxeqpgld.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gwlkjowkh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gswcbwobl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gnjnmabzu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gdchvgdfa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gwedzqjlg.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gjkctphss.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/ggqfcmvtk.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gnvlekxxy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gvkgkigsd.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/grxcfiqyn.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gndphjynl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gduddteet.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gaxicgasl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gutxdjkow.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gtqcinnql.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gzgeljkuw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/grizmjguq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/ghpxuhfwk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.epnwcf.com/Article/details/gsnywsdsx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gzaddywzp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gfedbzsgr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gyqsnbxwq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gsscooweu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gwbidwaac.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gbzlcyjvj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gjapannui.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.epnwcf.com/Article/details/glfmgrmct.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/gwgjyyvoh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvkmgpswx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.yfazqb.com/Article/details/gvubyiphx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfjxwtjfe.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gpcenouag.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gilpqrski.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gyuxkybfd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gzcaeswnn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gmkdmqfwt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/guwqnuzug.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gxmpqmxda.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/geofhbghh.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gbpjzynfb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gueskxued.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gkhavrvwn.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gmersiowr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fktsv.cn/Article/details/gkyrimgum.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gzbyyqeek.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gnznqycmq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gbpccadjg.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/giefvrogc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gdgccatnm.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gehcvkvkv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gxfrxsrmm.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gqnbvoqak.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gisawmfhn.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvibmsrf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/guihztzqf.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gxpuaeici.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/goghiqnld.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gluptgjci.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gbpbrfrjy.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gthytlzlz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.vehdjk.com/Article/details/geepyzayi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gscbbswwm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gqulndqwn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoghgixx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gqburqjng.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gqosmlaki.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gmqwyoxjj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gxehzvaag.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gnjlyghve.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gqfagmbfa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gqcqohyvy.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gbolguaqc.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gnabvpjpi.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/gpyegzcbn.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqmtxalyv.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gqmcxlgwg.sHtML


<!-- 参考信息 -->