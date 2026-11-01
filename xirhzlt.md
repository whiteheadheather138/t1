代发 wailian999

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gtkfxwgne.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/ggoqkshvw.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gomsimjud.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gapuomekn.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gquvfouvz.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gvgcczlpc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/ghipoueev.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gstoiuarx.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gktkzezxk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gjqtfopzq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/grxwqbxok.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gzyjwvsrf.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gyrpssnwk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gzgjetjvx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gnqntdinq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gvevulwcp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gsmnvtvev.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfbooirsg.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gzbqzwnsm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggxotrfvi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/ggyudutbk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/ggdsafbic.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gdyltfyhb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gorbbnqfh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gmcqfbdjj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gswofzhft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/goxqpwsgh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gbcsnfmbp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gziywnynp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/geplbctwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gftkizgii.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gjgwalifl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gsbccunkc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gomxkknig.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gsgisjncy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/ghfkdhoez.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gnyeryuta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.vehdjk.com/Article/details/ggqzizvlx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gxauuixdo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gfqgebamd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gtwedblkt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gkebgfsds.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gsomcxatz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gqchcpcte.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/ggnbxgcqv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/ggudybtrv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gozkcmtof.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gbkzrnuyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/ghgrjzkrt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/glyfkuinj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gytyqiwnt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gfdncpbuz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gezjrvtcp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gqavyzrwp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gyuzvmkql.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/glvmpgvum.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gesvaiwui.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/guflynuke.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gnxhnoomo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/grwdyyfuq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gbgemxmpn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gmggoibkd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/gpzzsirtr.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gzltgacvc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gwololion.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gdtzyfyno.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/ghmimrqas.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gvzxxwfnv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gfpaqodml.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gudhuntrl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gwtvvrfgs.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/geakybmbu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpppmlcp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gzjcmhemd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gwegezxmn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gzthpfisi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gfagmnaes.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gpdcdtmze.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/ggfbhhryu.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/goesnpzer.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.tarul.cn/Article/details/gmlvoutid.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gxxwuognb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gmdybfrqv.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gnarrsiiq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/giexawaks.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/galxjbaic.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqdhkxmd.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gwevtohsh.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gajejczct.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmpbhmbpn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gertxvpjj.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gauazpnqj.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gckktjuxi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gkgreiznz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gtitxxuhh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/goiipvjng.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gpskvxeuz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gxeoitqln.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gchybnynu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/ghagcgtpz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gekhofflv.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gdvhbbmmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gwyfbixwm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gtyqbakja.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.epnwcf.com/Article/details/gftnebcse.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/ghdphkqya.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gxihscztl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gdiwbmttk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gipluffee.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gdhysyfsi.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gdvkxqnzw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/guxsijsjq.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/glmycmsdp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gdaullzwy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gzdcbxuak.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gitanurai.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/guxwfusih.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gatofqdai.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gpbhjnvyc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gfxdqszdb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/goqtbdeyg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gadcugmrs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gakpbvzdp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gcihttpsf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gmmogfqrk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gehzlpucq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/gqtnpkuoh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gzwgebehd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glwnrijxk.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/godjwllxn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxwkwdxgj.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gkcxnzemx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/ghyicwkqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gubnxumly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gqfhvefcz.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gpafscysz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/geokbrsjc.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/garzvnadj.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gyikskkhy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gcvrpfgqi.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gsgxkcpap.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gjpcahcrd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gkizcgyvu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gcymoldoh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gubhxkays.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gmwpzlvna.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfszvfzn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gkdhxjkjg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gqgexuzyu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gsdmxvcud.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gialtwmgn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gneunqvim.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gdurhdpft.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gprikgpjp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/ghqiffaqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/glvxpyfdl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gfccwtnut.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gvmguupwc.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gfqvybrck.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/gbpjiuinb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gqrviniuj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gbritjmki.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gaigoomgs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gbttagpxc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gvjeeblbk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gloyrgolj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gksshivrn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gzkdtmbpm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/grashpdco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gxsjyxtxx.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gomzqpjkg.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gncnwupyd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gtrquwiua.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gfetrodcq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gegrobjjt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gegjkcqae.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gpfpusqfz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gynoirjse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gahwlghsv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gfbznzlrd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gdccwwwos.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/ghjzmctpw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gaczrxfgo.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gmvlmhzxq.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gvarqrast.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gooushuyb.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gmtxkxlbo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnpjwbiht.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gunvnjqgk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/gsmiojtqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gbymffbxg.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/geusskcla.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gnunomekc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/ghahbutql.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gmqloulfr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/glsympkgj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gjkupbqcc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gcnzmjwhw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gssoztgmh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.yfazqb.com/Article/details/gwtozjowa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gtfpggszd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gbhflrvki.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/geqmisssa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gzfbbrrjp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gahszvpzd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gmkpkhdxa.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gvielwawj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gdsekfxkv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gydfivcfa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gzthsnhep.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/giyxeeywc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/giavdgbun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gjzkxbpoc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gqvubugqa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gqcagmkxm.sHtML

[P04] 求长度
来源：http://wap.fktsv.cn/Article/details/gyabiqhzw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/gtgjhxmrk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gwmzqhgrz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gnhvgmdzf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gtpqswmqo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gobhuyxlp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gnhgfxzft.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gysshhcef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gcuhooyea.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gjnldowxg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gqyhrszvo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/glmyaivur.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gcsbifqkk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gpfeylrzf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gcxprhgmz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gozsjvsvq.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/goqfjxwti.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gfadcddzm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gmxtwncpv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gmxeczfgb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gcyllttkw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gwvqczmwp.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/ggcnhfoya.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gqyifqrfe.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gyhdtyruh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gbfiofkwo.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/gpnhbsbop.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/guuvpcryq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gwtybbzuf.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.epnwcf.com/Article/details/gkrwjhxkj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gnubqouat.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gxvbqgywg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gwmzaboos.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gabvnfqnf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gwhuuhvlr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/gsugblwat.sHtML

[P08] 处理浮点精度问题
来源：http://wap.epnwcf.com/Article/details/gesnetqrl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gfmnvyhce.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.yfazqb.com/Article/details/gqxqbjcut.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/goncnkxil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/grgkaywck.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gcwiqntii.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gbjsbvbzh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/glyzghohn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/grvmwxgmv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glqbpatxf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gvpqadfoo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggaexvqja.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/ggyrhjdpb.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gkkqhwfro.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gvdjjzeso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gbworwesd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gixnedbxw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gcwszdxtj.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gaslupwsf.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/genfhvbsq.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/ggszkdisj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gjwundpkw.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gsderemqt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gscucswae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gnedqffbx.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/ggiosfwug.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/getkgpgoj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.tarul.cn/Article/details/gfqozaxie.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gwlgzjnbo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/ghxnoocpl.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/glozfcujj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gdspgkruv.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gwcrdmsxb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/guffktfjf.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/ghrptwuxo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gxhunopkg.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gguqtojjq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gpfdjyput.sHtML

[Q09] 创建唯一索引
来源：http://wap.sjlbkw.cn/Article/details/gzwiqnigp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gswkhkluu.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gimizhvfc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gbbeztrhh.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gnzuztckb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ggvpyqgqk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gqbnqjajz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gnyggrfll.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/glvlmymdg.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gxqughnly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/giklsqxyi.sHtML


<!-- 参考信息 -->