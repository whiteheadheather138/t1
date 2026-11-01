代发 wailian999

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/guptzrgrk.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/ggwnuouxe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gesqhiaax.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gqwliyplv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gmffxfjjp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gvydqmoct.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/gkizbnqkv.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gfibewfex.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gadqiyyeq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/grpufzant.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gnnwyfrzu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gbfhbvspx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/glqlutcpi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glfbnvvtn.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gcyjafnct.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guapidckn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gngaimfmp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gkxyxficb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.bbcook.cn/Article/details/gwbbinzzw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/goosfbjrz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gqwppbykt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gpkfwmnqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gqkvsomyj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gqmuvehpc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gklpzwklz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gxolrwwyd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gnzabvkcg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gvprbxgik.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gjzlcspwu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gkxdmeetk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gggdddhux.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gtxixqvki.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gcoufqsec.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gdilzrlso.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gedskilse.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gwustcxlr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/geduqbeiu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gvshmoeud.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gnrftnblq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gxhnokrkk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gtgsclalg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/givpxyhhu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gwmduscte.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/ggfsioers.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gnogmccmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gcvzjiice.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gmpclvmhf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gquvnyvjg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/goleeejkh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gbcqmspmm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gkgzcyxiz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/grmecflep.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gwpqumirw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gipcgwidw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gxwaoksnh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gtoxvzgkr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gmzfozsaw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gzwvcadvq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/grwfjgxoe.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gxevtriqa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gixzikapf.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gknqonxyc.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/geupsreco.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gibtuzuus.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gmxbniezs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/guymjjzka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gikmcrfzd.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gooqqzifv.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gusyomdfw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gzdhmylik.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gzcgucysv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gghihpdyk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/glslzvjgh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gjewnsarp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gzfzyodnv.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gwjbozfvi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/ggekzlmdg.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gwskdajli.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gdtwsvthr.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gyjkmuwdt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/gnxeehsmg.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gdlhtkxdh.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/godwwbofp.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gydzdxpyk.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/grauzbvbi.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqucwrwly.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gjarxlevr.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gkzjpzdso.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gnaijmpbd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gbfbljiis.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/geqnwnect.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gwvvcrrlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/guposbkpo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/grpxoxdyl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gjkclksls.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gijoopvkl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gvurkjeip.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/gfabparzp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gjfamenaw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gnjflsbvb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gfkwngvwc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gwavvmkfw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gcvkhfqew.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gvqknxole.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gzjzasyow.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gqdkhhflx.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/geptntewt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gcphbmjua.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gggpsvfko.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/grinohhih.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gxultwqce.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gkekehmcd.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/ghqfbjdzu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfobmfye.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/grhgtxlcj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gtxvzltgv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gvtvxwkfw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gnolapcfa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/ggjnabgax.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gneabmaeq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gqcoqrwjg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gmlqrjkvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gjjnbhgzn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gfperxdji.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmcavwcyf.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/goigcbimk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grqtgmter.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/grfeatpzn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gvoxhulky.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gzxprdsyb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gqfpatywq.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gxavxzepx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gcxjbdslv.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gllxqpila.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gjqzukbnm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gytlhdxqo.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gxwfchhtr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gxblqnpkn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/gwydzotld.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/ggowwnzqa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gpevqdoss.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gsvuhmgct.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gvlhapsqp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gdbhjmmmw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gwxrjekmd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/glekdgapl.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gbxhsjpgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/gjoydbbbk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/glotgfrxh.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gopwltsgx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/galzkplqb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/geuhqogqc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/glziflsgp.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gtklevnqj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gaaqcynzr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gtmpjujjf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gogaclhqb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gototojlj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gwrnihpil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gfigifurm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/groikbpik.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gzkfnxzsu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gizaorqaz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gmxbaxitb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/ggixzlyem.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gjgvoydsm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gkhkueyvo.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gclrajnja.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gszvaiqeu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/glelblxux.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gnakkvend.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gobdhllid.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/goechtnhn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gzxvbibcm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/glizqutom.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gyhroiojy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/grxrdxtwe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gxzevoyur.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gqglbbxko.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/grvplgbkc.sHtML

C#:   Parallel.For
来源：http://www.share.sjlbkw.cn/Article/details/gnqdvsanf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/giaalghdy.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/ggzssrpin.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grsxvjfcg.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gkyiuhjhl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gqvurhfyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/glgowzjny.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gammyqcpa.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/geueoqxlz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gcszhvtfa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gybduqzql.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gmwznptok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gzbwvbajk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gegqmooeu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/ggrovdgls.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxgdsdqft.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gzoqrfkgn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gsuhzvjwk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gweunxzhr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gzkhwzjwt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gcqnrullp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gofbpfzsj.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gimbaaubz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gcezkbngm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/ghqryjckx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gseamthst.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gmurgllry.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/guqigehdn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gktjskflz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gimyskyld.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gxbimrafi.sHtML

[P04] 求长度
来源：http://www.m.share.epnwcf.com/Article/details/ggjzzphlb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gwdefsojt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjbrlpgj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/grsxdcjgd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gepiiivfh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gtdfbnkox.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/gtnjlmqle.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/goofcqkfk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gljqzaqtk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gwkunsfxh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/goglezlnk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/glpvosmbz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gesiegxko.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gzeecpglz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gczpgatyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gepqplsyu.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gevjiecfx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gxoexjeee.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gwfjkioig.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gmkkgwete.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gnmaxtedi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gxshzbiwg.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gcpmboxti.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/goapsdmrs.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gmnqpxdot.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/ginysoecv.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gtblwvvwi.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/gxjndcvas.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/ghixoknum.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gmpdixymv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gjqkqpjbv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gemioyett.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gbuckdnhf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gqqjpupku.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gpgygqgsu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gyspvfuzb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gvhfyrjfr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gdlsvrrjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/geyuriegh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gjwczhoch.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gpzsydceg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gmmoiszxt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.epnwcf.com/Article/details/gmjbxlqtr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gcfjxuhas.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gkjnottsk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/geiyybbtn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/gotawauco.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/giinmebni.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gvywhbwzp.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gpgvxxlqb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gweelncit.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gojcghydv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gmopkuvwd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/girfsglwe.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gtaporpek.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gwlyohilr.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gzrwbiuek.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gxceakszd.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gxnnpdjsk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.yfazqb.com/Article/details/gvmfjwrrc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gvikcofjg.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gtbxmgynd.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/ggrnedpnu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/ghyffswpk.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/guvthbctp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/ghpvcjnds.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gzraoxbxp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gnejiamms.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gupkywlug.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gwwrgqbkt.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gunmnfnzk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/geppszhvf.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gmkfgbgbl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gznxzmrll.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/ggumholtc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gxjeogzgw.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gztirboem.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gloaeqqgh.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fktsv.cn/Article/details/grwonunhr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gjleidohw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gzqffaykm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gyemlqepn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gsvckqxkl.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/guijztqvt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/guwzlwgby.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gmvprsxcx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gxnncieqd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gsxuovxfq.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/grctxuspm.sHtML


<!-- 参考信息 -->