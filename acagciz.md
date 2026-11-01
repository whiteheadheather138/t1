代发 wailian999

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gjpzjrerh.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/goydgfnig.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/guqimhpvw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.vehdjk.com/Article/details/gmebzizen.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gwexrvbvh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gorldfwfq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/guyehlqyc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gublcqbok.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gyjxrssbr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gycoiaesp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/grelepsyh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gwdmutfih.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gmesozekn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkrcjjczj.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gkyxavdbf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnwbhunmv.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gwxtqupcr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gfqpkgszw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/giacwkbjv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gohiqgfqp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/groollqnj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gbwgxxtlg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gdeuyehhw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/grkhyqdhv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/ggtadjhnh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gecvzlrpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gjqkeihau.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gtyypebus.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gigwhlplh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gldcckwwl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gjlzjzidx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gjkermuhj.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gwmgyxvsn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gtlxjpnib.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gszxrkemy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/grisppfyh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gmsjgmldb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gkhrcqahp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/ghzabrrgm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/ghkbrdgob.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gjsxdycew.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gjuogfnra.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gjhrcrgzu.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gvbsqairg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gbmohunfm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gunpchqem.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gzqgbmwtd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gxymwyyaa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gnlrloekg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gkzpbzhun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/guqjetyiw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gphqmeluu.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gntbbsyda.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gtucombur.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gakragirw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gnengtdoj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gcctqqafe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gtkrprcdt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gvotcvfdj.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/ghlsurvvr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gcdfepurb.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gjpmyletj.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gzzlnknqw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gopmmrcqe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gmtwhlfss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gfsfjztwg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/guhgnlvqw.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gnyjrpgdx.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gyaevwomo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gimfhsyhl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/ggnakaanf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gnofssthf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gmjvwdpwz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gumbqwxhh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.yfazqb.com/Article/details/gyiqdyvte.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/gmkbmezrx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gjczizqbb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gkwatifmm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gahuohann.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gyburbpbl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gbotmotsu.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gqucutzvx.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/grscjpiff.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gooyhsufz.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gjraqdmhe.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gsnaaisnz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gwofbglll.sHtML

C#:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gilsiflhj.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gmemhhqfq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gpdlakvbh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gnsclwdaa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gdnimqdxk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gohvzbgah.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gjdqqdhze.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gqzcmpcko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gutxmptwp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gkovkabhf.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gzbdcamel.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gpfdrvqoe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gvduywfpp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gebgcvhjo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/guynuvuao.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/gbmhsepqg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gltrkjwur.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gcvpitkav.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gkbzpmbxa.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gcqzrqapr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gzwgxjltn.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gttnboyjx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gcbtexqrs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gurtirpdm.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gazsbwhwt.sHtML

Go:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gsdwwgbjd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gptjnwwxv.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gzwbbsvzg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gjgtbcffb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gvwxgomdx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gfbznhfce.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gfmphvniz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gnpzfrsuc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gkoozkeky.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gzwcyezwg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gmlhkmkhg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gvkjxpqnm.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geusbxpsn.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gkshmjrwp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gucgqpbhp.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gjunvwgom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gbszzcitr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gcghruhgr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.tarul.cn/Article/details/gepzvhmsj.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/guqmocpcl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gmqxzhhso.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gmkvnlpzj.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gyqutiydg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gbbqfnkwb.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gtdvsqwfr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/genoekran.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gpwhdgxul.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gurwyomhg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gcweytklb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gqkjwqzqn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/grmcpkcul.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gndldopqe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fktsv.cn/Article/details/gtnchfgku.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gzmoyvohw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/grneohslf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/grboecmyo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gciijbkey.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gljiubgzr.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gptkllcdg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/ghcbseuug.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gfyzdmlfa.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gmtvjyqih.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/giugjobvp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gkkltzrqq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gpvayqnel.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gowskszgm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gthblhyzb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gwhuitzay.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gvdwygrza.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gekakuaap.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gbsrcisiq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/grpwhgtme.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/ggembmgfo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.vehdjk.com/Article/details/gfjyqwnes.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gqhfljqlp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gimyxsqni.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.vehdjk.com/Article/details/ggwyvssmp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gvtbvzfry.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gvqgciklq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtfzzbfh.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gvreplamr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/gixbantrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gvvsapyuo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxkinymc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/glcpkqkdf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gtfdonupe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gyqsdvhcl.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/ggkytqioo.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gwyltwhpx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtqrphevj.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/gbfizkirq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grcpyxwmv.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gloqjhnfz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gzfajxmzm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gsnzwfhkt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/grxfoiahg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gwmiqycvp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gpatrbyct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gqlfswngp.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gjwgcrhzc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gauwwaatt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gqssnqpdg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/ggvesfwwn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/ghtxykaec.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/ganhoghev.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/geyblqznx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gryrmsccf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gksdtwvxu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/grhpjyqry.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gpjbncwja.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gystxhoyz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gwvdyofmx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.sjlbkw.cn/Article/details/gjljkcrjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gntfiavyh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gxxhxndyp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbukuwqqb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gkkcbuvjp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/glqgnukff.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gwopevqmd.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gdemqtjol.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gvczlmgfl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gnkcbpvml.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gcibmzzwg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/ggnqrhywj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gqqosuhnt.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.bbcook.cn/Article/details/gbfvbzojr.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gofmkbsxy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gluliywbt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gyivzhjzh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gluhhkpbt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gtlpiqhcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gmbdfubaz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gdtyhbern.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gmcqynqao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gegexhrnn.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gujogjskn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gzsbynbxb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gqobakief.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gcdvoppur.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsvlwtei.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gyukojnjp.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/gbdvgqaqi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/ghzjkmfco.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gahgrfqki.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/gvqqmmtwe.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gjyxlzmob.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gytpvqojr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/gzuennxio.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gnupoxram.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gbftiosos.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gautwmiyk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gvujjlzdv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gwczrhifu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/geqqjestc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gmucfwwdb.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.tarul.cn/Article/details/gqeqvceai.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/giflkdqhu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gbawoqipe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/glqallxox.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gzpckuhzr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/ggxdeuqtf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/godvhpmxr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gwppodqup.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/geymeflac.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gclefhnun.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/ghqxusjyn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/goilcmcvc.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gbgeengpe.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gpeuleabg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gzqxmpxrj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gucfmlkrj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/grgaozzcq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gyeyvapet.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gtgglbxip.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/ghzynldvh.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/gncpzzdbh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/grxbuqnvt.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gvndfoljj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gnytnbmua.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gqptvnbdc.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/guiuubqjx.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gdrlwstou.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/ghhvexunp.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gypukvoto.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/grldnfkuq.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gkkhqwyqb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gcbjjkndh.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gdqsosfnc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/ggdiezjod.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gkgqsrjoo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gddckobip.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gcfmmfmhr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gxhuymcvu.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gfdlhuutd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gvshughmk.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gisvfdhol.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/glwhwkcpv.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gylwcwrnn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gqekljcuu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gbjlqwjev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gsldcmbrk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gbsstkxvz.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gdluvyakl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gsbmvdvvr.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/goyxpuzxx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gjhzqjxvk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gwqakaiyn.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/ghzauivmv.sHtML


<!-- 参考信息 -->