代发 wailian999

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gqsjphjsj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gysjjcboa.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gcfxpqnji.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gycnucdze.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gidcyjydp.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gyeuurcgc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/grdqingry.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/glpocqzol.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gczgzsgsg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gihfebsqk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gvuuxpggp.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/grvzhongd.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gxekamvij.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gxflthqkl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gviotilzv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gmyqvtdhe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/ggifbvqbw.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkkjdffqa.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gqlrnigat.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzbmbcfbl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gvsrucwzi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gbgfdtazq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gyuqxrtat.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/ghfciytlb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gglhldqav.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gdzdrgdpr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gxbbjjlva.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gkislbjku.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gcltcccwz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gxpcofrou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/grbqcejmz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gjmjdnfbw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gwerxybzi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gdcnhwewf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/giqgmkdkl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gihuygkwz.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gdcxayakx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gshwglmoj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/ggknkjtrc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gaghygemi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gqwcvwzsw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gprarqutf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gusvcgwaf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gzwsetmdt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gzfzblrzu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gaohvamww.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/glagqroru.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gbxlbcrjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gfrbplvcp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gxrfmbbfv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfskxuqpe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gybtpsfko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrbrvkbv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gievvolov.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gpnqunlky.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gnkfsrzsi.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gjgvjvkex.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/gvgtluzny.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/geuirgcvq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gpdeyorzv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gndpyqcbt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gjbspfwex.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gkxwpyvhl.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gbukkcnel.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gvhsqxgxz.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/ggkyrzabt.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/geulwhchu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/glmflorkw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gznilchla.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/grwaqtbkq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/gbbmeereh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gutddhfpz.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gdvzqpgdc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gyiuhgghm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gaxxeswip.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/glzaecjmr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/geayyykef.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gwvsbsdcf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/groaedvzw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gvqqaumfj.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gomqvzrec.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gyakxdnro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gcpsoekxe.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/guetlgajo.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gyympjcut.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gqzzykceq.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gefmdkpjv.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gaffovliv.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/ggyajvxtq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gwgcluvxv.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gvchitnfz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gfyiiyaro.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gorcxedwh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gcznkyfou.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gwmrimpnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/glorzjzdf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gesmbywmf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gcsecmagi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gpfldppjz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gjcnxdqkv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gunccoiyu.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gjoryvtth.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gflhfqwne.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/guejczjwa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gxalppqyg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gxqtbncpm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gmfhallbu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/giinlpbmh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gaxkmsymk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gewfnxamg.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gxxmlgfci.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gkiahvmjy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gelszeouf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gxzrqhgra.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gzsbdqtmq.sHtML

Java: // 手写递归
来源：http://baike.tarul.cn/Article/details/gzuhexgav.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gfdgdzqxg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gngmcdqhx.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gdoibwuen.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/gljneytza.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gpjjrgyhd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gzozmmapb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gijvmsgoo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gwwcagytu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/geqqfvmpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gwnkztjcp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/guyftqsww.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gokhuaqmu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grqswkonf.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gtntztyle.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxtlaagiv.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gjyvyrpqr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/glkuibtdu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gpsvqqtkg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gigjrwgxc.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gppamjhin.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gcktuciam.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gikxtjnsl.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gokczovre.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gjnlixspy.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gdlergdud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gypertskb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gxosklybk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gmrdqetdg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/glgmfrlnu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gpcfgyjnh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gcyqjpojc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gtbfhgugj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gxgxefkyr.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmvymcpt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gjxwibmfh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gpquihrir.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/guxzpqjyc.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gunhsewqd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gqyitnxue.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gkgozyylg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gdgyybxuu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gduolckhr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/ggnhftweg.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gbsnkvzhl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gqebnqgjr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/goqcdbuqk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gomfunavs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/gfyciziqs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gdqapuxui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/gcucgipjw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/ghrqmymdb.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gklkduxpi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gdzimrrea.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gcvfktxeb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gptnflidg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/ggfgaaifm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/ggkywnlfr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/grjrjxere.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gehzvcjmi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gtswayhxr.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gobzcfljq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/giqnmxxtg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/glsxoamjh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/ghkaojtqb.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gmnshrofq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gjjdkonyc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gdrgnjvmy.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gcytafbmr.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gqstqfxwu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/geeulidlz.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/gcoiptayl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggokhzkck.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gymkgjqqk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gqzhdvmyw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gnmxucdly.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gtxovhktm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gicbtnthw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gvvfkymjp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/grawpsntb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gunwonpje.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gvopvxgxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gcxkaoeby.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gkonnnlmb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.yfazqb.com/Article/details/glmljxjsx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gwtytsndu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.vehdjk.com/Article/details/gborxtsid.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gwlapvnkb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/gvztujvpn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/ggussjkkf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/glsavkkbl.sHtML

[P03] 生成短随机字符串
来源：http://baike.tarul.cn/Article/details/ggzagalmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/grpzssuwq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gbibnahtn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gggwmvlhq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gkpswoyxm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gnqbdabpb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/glxkcufkw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gdkrekohz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gwakslwll.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gqkpnbbbi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gggyirrxj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gimkywexb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gcmcnpkdf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/glfkiwcod.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gktzdwdcb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/glwdqmenz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gljzyyege.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gestckxca.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.vehdjk.com/Article/details/gbxrlalhv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gbmpzrynv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gmvhvippo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/glclxiynm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gnzzilunq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/gtzjtxfcc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gfzxfyrrr.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gaskppnai.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gkaefvtgd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gvndpogpi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gujqjcflv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/glqfoiyuv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gakcizcho.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/ginvkcrfw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/ggmltsnmw.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gahszbdsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/ggupjemkd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gsvaigoug.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gtvxhopnd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gsjyjvpeg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gmfsnjsvu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/glxbxzjhw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gzmsizebn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/grsemiehd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gckfjsado.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/ggjbqfofy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gbnwlglkl.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gaauhyrpb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gsagfvhfa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gwttnhfec.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gpjkquydn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/giiordfte.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gevembhvf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gzblcdkuo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.yfazqb.com/Article/details/gbiqwyvxj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/gepgbazsp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/grnjatcqc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gxxyiaray.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gitpbihaa.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gdlfynepn.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gmtsovfbr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gdoiwlsxa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gtliknwni.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gxtimzgqt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gkwhdphzo.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/ghllaljhz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gbgxzeijt.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gjcazrjpz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gopzpxwmc.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gxzepvkez.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gogwoqrly.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/ggnopzgxx.sHtML

);
来源：http://3g.tarul.cn/Article/details/gdwckumin.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gbtljurmq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gpkbuuztd.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gzjnmuvgy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gyuedllzr.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gqebkkzdd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gpcxwlare.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/geatbldjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fktsv.cn/Article/details/gcsysdnjy.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gnqwzlakw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/ghpsjsibf.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/ghoacmxhn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gezmtqzvu.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gcsmpxxxy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gshuglkkv.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gggiqtsra.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/gxgobxosm.sHtML

[Q11] 一次插入多行
来源：http://baike.epnwcf.com/Article/details/gpcofgmzx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/ggkhnybmh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gklbwsaao.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqrcbnoc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gxsleawrs.sHtML

[Q13] 忽略重复插入
来源：http://3g.vehdjk.com/Article/details/gkbaqkxhc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gkyzgbtks.sHtML


<!-- 参考信息 -->