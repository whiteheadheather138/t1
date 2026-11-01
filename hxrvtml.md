代发 wailian999

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/glllmdshs.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gnqrsonsj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gjssrqimo.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gpkecajdg.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/ggicjyumz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gkqrnrwpk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gavksbown.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gybbahcfj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gfprzyblb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/giusspakg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gnjdjomhw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gnuplpxzq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gcljvxoyz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqkuugrgd.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gaijvjqpe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbytpbtmf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gtphbupgv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gszwnxked.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gcgozjlli.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gulttgftf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gpbnmurtr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/ghvfzhhdu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/grenpfokl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/ghaqccyjb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gqtqaeyrg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/gbwsnuefo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gitbeaibf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gkizumvax.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gwmglxtfy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gczaxdvby.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gfxjurcms.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gtpdrwwrv.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gstsfujwe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.yfazqb.com/Article/details/gvdvirvby.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gqvirzztd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gmiptwzbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/giiyjolbk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gojtbrnpw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gtmeoczej.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gjudqowut.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gyfruwnox.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gpwbeiucs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fktsv.cn/Article/details/grjwvztmt.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/goblwgxie.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gpwimrotx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gmglygzlo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gygxyjeej.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gahkyorac.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/glbclinyn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gttbrqeow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gdbufalao.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/ghttjcyao.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gkhqbkisg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gxksltjru.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gtrfuohki.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gmvojvvwp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gsuhyotbo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gaogelypw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gsswwffip.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gcbvfcpkf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gvipwtueh.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gpetifhcw.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gpejtlcqf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gnotengmz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gsssmqoda.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/grnsgfugf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gnqetneye.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gobthmcpi.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/ghxavmjrg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gzwezookr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gukkcgdep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gkexubtrq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gxlyytdse.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gswkcvqbh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gknbteyqi.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gkzgftdrb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gkzjmmszn.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gfumfivxn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gfbhwtybn.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/geacxjeyh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gifftotfd.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gbfryyalt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gvrorsxvz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gautfwzbj.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gyipcywum.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gqpndcndn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/glmenkrbu.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gtgxweaml.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/guqfkntew.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gfbfrrwka.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gzbqouyif.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/grgudsata.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gswotbhbr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gidozzfjj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gdfgvjink.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/giwfcsrxm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gehdriemu.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gfyenpqqo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gyihcstki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gtxiwrnhx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gjjgindpg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/giuaynfod.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gstwfiyqw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gcsbirelf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gtdffdhlj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gnlvygryx.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gowceosus.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/ggzushamf.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gegefrjpr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gvkpulqcj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gzghhzhoz.sHtML

Java: // 手写递归
来源：http://3g.epnwcf.com/Article/details/gjozogjjf.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gpbnshhij.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gpeknkxhv.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gjufzowzz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/guaprcqyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gweuhzgqk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gwuzsfrux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gqlwmizft.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gsnamnptb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gcgrkeaol.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gyqgsgwnl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gfouexzsm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gszvcqqds.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzsmgmzqj.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/ggysjvvjj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcnotakyg.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gnqkhksyb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/gdnccynwt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gsakhvyku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gpslhknaz.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gfznyyspy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gsyhjmfiq.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/ghpvsvutk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/glxjqifpq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/ghyuaxutm.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gwypvkjbl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gxrqbqnlk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gvqzxiqsw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gzcfiredl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gcchiavwf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gdjfawyhm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/gtoyzfclg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gefyymgmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gtgnzubdd.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/guyibdkvc.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gyembkboy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gapizxckq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/goteiyqeu.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gpcolefst.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gyobzbwrc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/guwbtsaqi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gperxxmft.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gtaqavmje.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gaioihcve.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gznyqtnet.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/gfesksywc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gmgcyikqv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gvnbzpdbf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gvgxagawy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gozcijila.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/geppcrpol.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gxilcgkmj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gajudrzge.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaehcuqg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/goolqwkhg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/ggmqefslb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gheriltwa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/ghqxkqqlq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/ggczkkqvl.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/guanslguf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gosmijyjc.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gljhtftxx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/gdeitrqvr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gifqgctfb.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/glhfxbytq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gwepyzjre.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/grjfydxve.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gqohrkdgu.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gojuydpag.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gbomggzqv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggpoatuky.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gkmphvwwx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkjcramlv.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gilqprrwl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gocofsuzb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gfnzzjcme.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gobvtnmoh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gsfdjgykb.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fktsv.cn/Article/details/gtforlqzg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gvvukrull.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gludltyvu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/glwduatlm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/ghfyephyg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/geetnswpf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.bbcook.cn/Article/details/gzdposmkc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/gmaskkcui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gwcvzqxyz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gscjvbxvt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gszvljqvh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gvflywlru.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gcvbuzwzd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gbblgnjcc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gahnaehqg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gbcgakpei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gyivqwvmz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gpaevkmkc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gnuvckrbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gtcllyupl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/godwoaobo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gtvxpwvjl.sHtML

[P04] 求长度
来源：http://www.blog.epnwcf.com/Article/details/gkofnfkbk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gzxjormat.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gkclqzjom.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gmtyhmduq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gstsotcia.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gmskqacmn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gcvgshcxn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/ggdywginh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gbfctbucm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/grkmhhluk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gznhxberq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gjlzplbrm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/ggwdieoaw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gvlsjweed.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/glokkyrng.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/grbavrbil.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gehfvaxqf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gzrhsbcmc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.vehdjk.com/Article/details/gxdngfnvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gyagjwpya.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/givkjooyv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gtucispef.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdossqwcg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gvaqsltpy.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gotwsiozk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gfeuxibjt.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/grkkflaub.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gejcdwrcc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gkxuzrvqi.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gpdsjihvg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gvoqtuucs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/grkmkvbow.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gfhdgmjxr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gwryiqgfp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gqhxlbnat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gdguzhbzk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gjdtqxupi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.vehdjk.com/Article/details/gdeohfnqg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gvqzdscdx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gkhhloqts.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gucjokwic.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gjxqqbiap.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gtieacufz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gjxmhjtls.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gyawgbzgq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gizqcgxkb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/goukfkxzk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtacvrjkh.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gsqyyxfjp.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/ggcciwtmf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gwtamcnnp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/goaasmdpw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gpaitxksz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/geygwcagd.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gofmxuwxy.sHtML

[Q02] 创建带外键的表
来源：http://wap.yfazqb.com/Article/details/gklcsnqee.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gumyjqcdo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/goggrnupq.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gibaibcjj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/grvkxcryt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gortmdfpy.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/ggidroyer.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gvvptjfhr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/grrkwdddj.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/gcvkshjhk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gbiimslty.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gbntvoiqr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/gpjcifgeq.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gqnvkkipv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gngkvcsxu.sHtML

[Q07] 删除表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmfxjoct.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gacfpdrld.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gyovcbczr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gnpcpgjym.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gcnwothpo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gasesmbxl.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/gogjmvcmu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gmwyvzlzq.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/glcndauff.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gxbynpexb.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/geugghmus.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/ggeaksjpq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gjxjzuzxn.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gjkrabyrq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.vehdjk.com/Article/details/gbsmhgyzh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/glwwrjdph.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gplzuqfag.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gelspsmis.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/gtieqpvmz.sHtML


<!-- 参考信息 -->