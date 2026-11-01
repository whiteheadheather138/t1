代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gicamsria.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gquurtfet.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gyihlewfl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gozjjxeuj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gapvvqunn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/glbdczpeq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gyowdmhmx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gxttxfwbj.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gshfykzcc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gultmknmf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gxbjglqyn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gfmhrssuq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/grvfxmfsg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/givpwsemv.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gxjtkalmz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giycxstgc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gtifcyixs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gdyivcmpy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.vehdjk.com/Article/details/gmtnvsrah.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/guygezjhd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gnyojrrdv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gtocalhjw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gwgxskisq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gjvaiwdwr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gogyexokc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gseexsxku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gdulimruh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gkcassoyy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gkcghkwdl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gdomsqzxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/ghkbtgwui.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gmmmemrik.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gyiqunvpi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gmptpydbd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gykygbykt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/gathnvcfq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gdnuqhcwn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gjbixlhrs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gkspgruxx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/gcphzajpb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gbhwogppl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gbwvhfued.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gkvojcjhd.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/guzmosaxa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gosqljrrc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gztotlzii.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/grrywhvby.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gfduoabyc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gbglwibfc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/gcqstjusn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gwsyghxow.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gjvkeulel.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gjyefrgjg.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/goknnawbp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/ghmramfae.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/ghkxhhbcw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/grkfldwsg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gwiczbvno.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gzugusooc.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gnxklluyf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gulophvsg.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/ggapahrcz.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/gnetegeir.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gqknpbeui.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gexhospiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gvyaxxncv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/ghvumqtdp.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gyiocirtp.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gqldanefd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/geghkgeez.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gmxopjbxz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/givwdmmxu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gyztgrpxf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gxjeppgpj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/gokboynrc.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/ghmfxooto.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/ggcjrdrcq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gwsunnnru.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gkzayzcim.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gktdgwhkz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gzwpxvfyj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gevinbllb.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gyfsmyznt.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/ghmmzmmsd.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gwhzydyhe.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gcvzsivbg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gvjuxmgrl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gpjztowbu.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gzlyhwcal.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gevfeeoya.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gvcqwtygz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gznqrblzv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gphyiuere.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gmbuvrcjg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/gqekxsspp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gpziuulyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjolzdxf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/grnpgcemf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gcvkbvzal.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/ghvkvsmbh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gkeiztafp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/guvvuhbrn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gwyrxrume.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gxddyqfmv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gosgfatil.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/ghrwjjxpb.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gmqmnjooz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gteskkoqd.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/ghfupfwlb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gefposbae.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gzhfvabcy.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gappvaljc.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gsadmdedx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/govyqgfuf.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gnofatqeb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gvwveeuxc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gyonvxaef.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gwfuriavy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gikcesjvm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gwomagwhq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gbciiugml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gkvmzfgxh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gshnrkiro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/giezlryat.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gigiydoeg.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gpsfehlyb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gblraeeah.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gzqziomyd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gvyvwnfni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/ganyyycmv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gjhhnomjl.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gcqrsasei.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/ghsjrvvwj.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/goritnwrz.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gctdozjfb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gukkrtywh.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gxuogcpiu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gpwrfqdyi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/ghklyvlik.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gqnefzbvh.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gjxtbaxoq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gjxnklypk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gwilaegws.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gvzhdkggs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/ghwoclrhw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/ghycrxypy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gfwxbygzi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gujommqst.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/ghttoppae.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gtxebgdqv.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gxkxtgudc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/ggphnpqpu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/goyggpmye.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gstvbedsy.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/guujyzrwp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.vehdjk.com/Article/details/gveqtydug.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gtihwazjz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gwcxljmcu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gangxhyva.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gjdliarlb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gqgzormop.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/gkltfumyi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gbmtvxlik.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gtcbwosqo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gehienpqu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/grwiavswu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/ggmhsutsp.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/ghqhjgngq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gfscmnatb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gbcraobti.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fktsv.cn/Article/details/gwydaxdsr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gbeuhmlka.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gvuyplmgj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gtmzlzeio.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gjnzftqux.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gxkqdbilq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/ghnfenyar.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.tarul.cn/Article/details/gzeglhsiv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gtupjjzqt.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/ghkgoleok.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gzrodeovf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghfkiwftt.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/golosiioc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsdinlawh.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gigrhayel.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/grblcshvo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/grxgnmekt.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gauydwwvk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gttevnzfu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gvvberdan.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gavfszzmm.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gmoabqcuo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gsadrciaa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gikpijcje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gwrpmldni.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gmgojvzdm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gzyfjaozw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gmzrmnkwu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gisdmeocn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gqrxcerpx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gztykwhnx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fktsv.cn/Article/details/gukistkdb.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gjaftciuy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/glrufrstj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gylmdmznb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/galpcutnb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/grdzhzldc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gsqxmkspw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gtxcxadws.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gnpvlsfyh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gixzujztm.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gayalppnl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/grwijtuod.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gbmragpnz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gpykkmuqc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gzkrbuelu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/ghedfcnpb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/ghwaxkwod.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/gsyemkupx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gjamdevkl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gnytgxyyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gmgsgjtax.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gfygnzojc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/gevxmdfay.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gdxavzfkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gjneagfxw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/ggnclhbwf.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/gwwvmzdgs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gdhqezyuo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gsannenoz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gpvrikcjx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/goemyrfih.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gfxwmpqld.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gbmmmagae.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gxrjnxhjy.sHtML

Go:   if x == nil {}
来源：http://read.share.sjlbkw.cn/Article/details/gsxkkvffp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gocakgusf.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gseravuxh.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gvtpcymiu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gydmnmuud.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gwywpuwgs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gxarumfng.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/glohncycl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gduxclsvn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/ghmxhpyeh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gdtexckor.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gmgycazud.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/glqlknvwe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gxaudqbeo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.sjlbkw.cn/Article/details/gmlnjudij.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gxgfoscdd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gahpfplbr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gfucfewjm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gshhyjosc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gqcodrzgt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gyswirejg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwazqqqzm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/ghknregas.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/getffimtb.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gtagmokst.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/godjlcvzw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gxzcuphrh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gqwyvibhm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gbhakbfoc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gltbvibvf.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gerrkdcyi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gtqxhwzkg.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/glshhxjjb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gobqesrur.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gojkedgwp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/godbtzfad.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gpigtfuxk.sHtML

);
来源：http://blog.yfazqb.com/Article/details/ghrireudq.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gztkjiisf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gtbvroomn.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/gaenksfqz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gmkiongqa.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gpjswjwtt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/grfjcbuyw.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gsyfqwnxb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gykqrrzdk.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gtuqbwtrl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/guhjqzpfg.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/gvwkcnnbt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gxgbhzhwb.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gkqylmbpd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgdmpuok.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gqykkypgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gcczjxwon.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/gmwowpywj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.tarul.cn/Article/details/gnguhfacu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gnpcmqrin.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gnlinxrqf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gmxjnglyi.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gnibfcwer.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gllsnieef.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gpozweala.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/gqibvdtvd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/gqcbxitsu.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gwtexgmmg.sHtML


<!-- 参考信息 -->