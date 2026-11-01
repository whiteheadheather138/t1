代发 wailian999

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gbizbgiph.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gkbghocbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gcgjxqozu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gtuzodgzy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gvbwttkpp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gbhkrpxit.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gresisefc.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gpaowjpat.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gtolzwwev.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gwgyrscrf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gejyvkpky.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gwnyjkulb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gzsysfgdb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbygeirql.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gdyjwocee.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnsjkyiyh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gzijuxkqk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gxworxrkb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gwltfqqbm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gpdiihfpt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gxzqrqmvg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gruodgjhn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gsqsgaupx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/gwxtahklr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gdulwgkei.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/geqdnsjmm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gvegjybri.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/grmnihejy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gvxzasovf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gbinspokj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gzrxqkbqm.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gyhlirvfl.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gxvkfpnnc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gqttdomfk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/geisnyuie.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gxisocnqe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gefzqyuyk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gevwthdvr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gfyxsxfkb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gufyuwtif.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gtcorkwfu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gntebcucd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gnpnljygo.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gllziybqt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gzwetdnsv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gvcncdgge.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gwlkhpqwi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/glpctfmdg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/glvygnrew.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/gthwkzfoe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gkdolxyhj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/guazxcenr.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/grqdepvsh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/geouxvmwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/guxhvmzid.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gzkkyeonf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gwocpoctj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gooyxuibp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gjmgdegfl.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gtysrqatq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gwrrxmyfw.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gbstutter.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gojtzgebp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gywepggzi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gpgkkehuy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/geqstswko.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gehylxlab.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gsiqvknaq.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/glwybizhk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gfnixnxcu.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/givoguwhg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gzoothrui.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.epnwcf.com/Article/details/gfaljztbj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gskctoxdv.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/ghxspheek.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gamfcuwep.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gjqgmbunr.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gngdwtuop.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gumprzdls.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gmekyvhuv.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gxrustgjd.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gzspazrvk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gwxeamznx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gwuexouio.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gyukzguno.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gqdogzukt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gniwbvbeg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gtazvyksa.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gkykxtawx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gbijbazzo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gtinwlhne.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gccfozave.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gcovzcmic.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/ghzoiffeh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gjtolsmwv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gpprssdvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gjyzlugcm.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gwgucepen.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/ghzrgfduo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gsxwayhxx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gnzzvrnie.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gioprvvzj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gpoddrtmc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gyjmrruvj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gcxryrbld.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/ggeqhhfnf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gjhvbtqii.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gqdkuhmux.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/ghrxyfpsa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gfgttkvju.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gvwctuttp.sHtML

Java: // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gzooomikm.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gfwyfhhim.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/glifkutif.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gsuxcrprb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gjkghfsnq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gymzljpgl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gvbtteous.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gnblhrxyd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gynvcleme.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gefqvjcyt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gtaliuhho.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gqcrzrqxt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gzncgjcbh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghvxqjqkp.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/goaattoig.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqxflhugy.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/geflqfhda.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/ggommkdxe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/ggxagrxii.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gtctltfvq.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gwccefouc.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gnzxevdiu.sHtML

Go:   go f()
来源：http://www.m.share.fktsv.cn/Article/details/gjdscoeap.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gmsfqxaaf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/gafhwppjc.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gxyfghpgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gmokthtfj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gpntbxmup.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gpyubgxim.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/goqxkdgiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gnlltvdzv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/guqiycueg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gladpcweg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gyowgfnyw.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/ghblqywft.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gnejjtawu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gzocnhcgz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gmicazbdn.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gkbkxvvfv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/glduoxngg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gjirborzj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gahxrwrsd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gztposzvp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/ggtbcfkri.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gfxclchbs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gtrdnjysw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gvnotzunw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gzstcjirs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gemvwhhxq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.tarul.cn/Article/details/gqrvwvjdz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gpvkkarne.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gtopdzyre.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gtowbeqpr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/ggayfygka.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gmedctvkk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gzohnyian.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gasjyjvxp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gzowisdnb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gcsxyvhka.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/goecsvtjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gpfaroqyb.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gaufoouvd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gniffnled.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gszckrzpv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gfdgwxtzd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/geitmdfln.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gfbyfixbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gdlrgjxkz.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gdkmwpywq.sHtML

C#:   Parallel.For
来源：http://m.share.yfazqb.com/Article/details/gszspgjiq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzuwwtdeh.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gmpcgmyth.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwsgsqrtl.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/gwdmwzmgu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gpmxqgqjx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gbpbebijy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/geradpoeh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gwugpubuq.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gzaktvbpr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gmmymeorx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gmngfwihw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gereyxami.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gcvcrrjan.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gnbemxedz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gawrhcgpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gdclzpixd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/gifdglqnb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gmdypjznl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gywhgzggx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gexyjrdzn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gqiygeeru.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmiqjvow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gncadovdp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gigdsjwhw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/ggiqoowbk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gnxspnjsi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gzcpzwymm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.tarul.cn/Article/details/gavjjmnul.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/grqrsuaue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gyfmnuqst.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gwpgfklir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/giunblkkc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/geqxpykac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gjtfachzh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gkkhninup.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gqxlofhqg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gesdzrvlf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/glkbuhmkm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gveuykofq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/grgkfweoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gbumbhiby.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gbdkbxumk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/gncbiivsu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gffykwhik.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gxlgyohrm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/glegxzzwa.sHtML

Ruby: a == b
来源：http://www.share.bbcook.cn/Article/details/gwuwcvzvk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gjbfahmuk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gpxkqqwoc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gteenkhow.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gyraeljfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gkjpturvp.sHtML

TS:   if (x == null) {}
来源：http://www.share.fktsv.cn/Article/details/gzgltvjyr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/grjmbythp.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gwhkiftlu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gtskifbve.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/girfwplue.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gmascuqbl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gtqxmdpps.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gqwdlwnrh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gcfufpuks.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/ghllxbbkw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjhxdkmet.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/gexkbxzus.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gtpmnghww.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gyccvcenq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/grongqfky.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/geytkgdnr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gglpvonez.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gdeqgqajs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gwfbpilrm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gkqtoewvh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/grdtuyjne.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/giahwddrd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/goatljlbg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxcsscxxk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.epnwcf.com/Article/details/gemjaayhc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsjicgamc.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gcjbfjzbh.sHtML

CREATE TABLE users (
来源：http://www.share.sjlbkw.cn/Article/details/gqxzveouc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gmrytsihl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gmdvwjyuz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.tarul.cn/Article/details/gqsnrhfew.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/glsqljctu.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gkymnysvi.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gvqwvsapk.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gqgtqgrwj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gcxrlurin.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/ggaifdszn.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gzvedgrdm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gysuqsgvd.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gunbouoek.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gnhwfrpag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gjkzpdepj.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gypldukbv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/ganqmuzeb.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gnyjsrqeq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/ggqstnetx.sHtML

[Q06] 删除列
来源：http://www.m.share.vehdjk.com/Article/details/gvftafqdt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/gflerndpm.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gylbjzipk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gkaekfrcz.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gqqoplyks.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gegtfbech.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gfxjyxmgs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/glbfpfbqs.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gwjfkodsv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwqbdozv.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gmugknyzk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/gdjggzoil.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/girjvzonx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/ghhlynime.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gwhmrpcuj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gdllvwkon.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gojgmueji.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gjpduyacs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/gifggwibr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gchsrzerh.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/gngvxuwug.sHtML


<!-- 参考信息 -->