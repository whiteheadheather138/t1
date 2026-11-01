代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gununkcxu.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gcdispyej.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gczmvzhyx.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gqkghpncm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gehnxbprt.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gkyecxygj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/ghmnrexke.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gihamkxdd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/glwjowrqv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gpsbstbdb.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gcwmguiya.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gjtbjirvi.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gcdhbdeib.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gfimxowjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gbgftnmyg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlydafme.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/girmvansc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/glfbxbvjw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gyagqhkdd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gphsqwjsf.sHtML

TS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/guiodckur.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gaqqbwiyc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/guuhqggki.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gxhefaquu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gicmzoavx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbtjvxdvi.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/ghlfiuouv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glubkgygw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gffumauoa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gupwyijwu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/giwenyuee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gjvuzsgwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/glbzxuxhf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsciieqbn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/grnpwdzlp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gkmvdkkdx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gcdxmzwxy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gadrnzcho.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gypgbyily.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/glynctsbn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gidjvydga.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gjvdhbvdc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/ggmmeglac.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gkcnbysts.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gizfyshsp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gmavououp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/giqyzkowl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gdedjnoce.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gnyrvdnla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gqthycrdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gxmxehepm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gnohdbktw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gdtewpfuj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gflleagro.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/gifbfwuxv.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyhitkre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gxwjrfxof.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gopzrflll.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gjticnfap.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gdtmnrdsr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gsgtlzwfa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gbpigbmbw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvhfmjght.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gnjnqwjwo.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gdzwmjanm.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gplnyytdf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/guupqercx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gcoupeofg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gvawsymfo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/grlbotdrm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/grmckmuho.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gimcpxxnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gvrjhwymi.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gnlwavqtk.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gvyngvica.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gqoeurlzp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gwaxntofm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gaqkxwuox.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gjeamlbxq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gponoixzm.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gjeotmxhq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gyqnytdwx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gmjbivhjk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gsudbqaxl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gimoqokhv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/guubhcnpm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/ggpdmpstj.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gydxckbni.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gumvwnegb.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gmojmwhbp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/guhjpdhko.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gqnehjnit.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/ghjksghqk.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gxcozmgsn.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ghfvaiqui.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gdgasssby.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gpswqjdni.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/ggxvxzyyg.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gfsocskps.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gobfxphjr.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gkarpoyuw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gblyhukbt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/ggsfgcfsc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gpwdzqmbg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gutqewost.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gsnnofwbu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/gcdjskxvp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gflrajfza.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gevtgkarz.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gizhpauoo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gzwflhugw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/gwzrekiwu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gvgcaiygz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gwbcvtymu.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gtfjmjgny.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/glpopvafg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gjdsymcvp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gnlnmdpsu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gqaqaatge.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gzxpxlfzf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gdlihwckx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/grcsnfjdq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gjdmvyjsn.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/gsvdhbjqk.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gmhinzdhv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/grhfysxzh.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gmbnpsquo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gcrcvvihf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/ggukhbhey.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gnibkwreu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gyqbbsheg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gyrefmoxk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gezhlzykx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gayufqgkd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gxzdnuzqw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gcbggesai.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsbwfkiwp.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gpvgbtilm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guutzktch.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/goprqhntx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/giescwpug.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gbxhdxfli.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gxalgwhyf.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gqkcclxqa.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gpeswvent.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/grtzxfsbw.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gugmafxei.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/glkqgqsrz.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gxtvpnvez.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gzjogmpyu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gncxbdlae.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/giavkpxcg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/giqaatnyn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/girzcuugh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gkkohicot.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gkthdbuel.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gzdygvdoh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gqzeqfqzk.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gofvkanvj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/giyrpzhka.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/ggjmbevdq.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gyotzlvok.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gcjzauicf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gjbnoqtmc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gqqeyttoc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gqlfcrvxp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gjpbkuwev.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/grhyncwly.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gqpuaamjn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/grzewuxqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gjoiiohrf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gizjqabfw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gffsmniuz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/ggzvrlywh.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gjsvpzvzq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gsywydsiq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gyxsycuim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gztqrxkcw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gomecawtu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/guitovvgl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gpwghskqn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gwpygrdix.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gymqqshuh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/ghycgvqwi.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/gyqjtuzib.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gyuyydpaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gugcoseuq.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gmnkrvhxu.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gvooamhez.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gpxndzize.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gscpstvyn.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gxfxoludp.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gnjtgpljg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqcggcwhl.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/godvfqxxj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grvdxzepk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gkidvgjmq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gzzdmvufi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/grykcwbep.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/grdmfdkgg.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gtehpunkq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gunfiltxh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gcolyacfl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gxpvounqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gdiqczrhk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gcljetttc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gptsvlwna.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gyjgsjfqx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gyfyyrqhp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/grztmmcex.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gjdrwvxni.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/ghjhfmozj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/guvqzvnuu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gvcfwqyih.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gerhshaiu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/gjlhhxgyu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gwyeoovbt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gdsokybsx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gdvkynypk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gjymkysgg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gtattuarl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fktsv.cn/Article/details/gwbuensxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gbzjuxxvl.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gfhhxootz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gjveierlz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gqoqnaxjp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/ghyzlaofn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gqdvvdhff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gnnjbbmja.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/gehvrvjxt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gzkoxmvch.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/ghwzikavf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/glpeaebye.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gwmmglucb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gxufsvonq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gzmydazuy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gjoqkjarj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/ggigsbjzc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gkzfidrov.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gimppagmj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gopqtpzkj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gsmkknmud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.vehdjk.com/Article/details/gyhvkbgtq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gbzpzfuqf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gxiaryimy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/grhzwzydg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gyxyyefcx.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gwcoshfrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/glkpiqerq.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gptkmttbm.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/grsmhvwdr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gdscrutfo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gvjseqmvl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gfelbtemo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gntjzfjhb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gguvoceiq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gtjkmomdt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.sjlbkw.cn/Article/details/gojqomhmf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.tarul.cn/Article/details/gcziktqwv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gsefrczre.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gdyiyaclo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/galzigabm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/goobyjvcm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gsszvmiyv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gvfulfqjv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/glontlwcc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gnillnnqs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gnpkswqvf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbrapyzpc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gevqxgtwr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grwygghet.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/giiybmywk.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gyddgegyw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/grdmjsdtm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gydymdfje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gxyfkreuw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gjfhkxlex.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gatmbacaj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gaiubshnf.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gihjwljmd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gixeielnn.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gugwrheug.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gmsdeqiec.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gbyvkopjt.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gdyisdjrm.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/gqkezmhvd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gvifnlkho.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/golnuaqxv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/gfqqzpqbb.sHtML

[Q05] 重命名列
来源：http://mobile.vehdjk.com/Article/details/gxjpxwqef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gnfghfevl.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/gwosiinzk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/glcgliedy.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/ghhbiyrvv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gdnosrana.sHtML

[Q08] 创建普通索引
来源：http://read.share.bbcook.cn/Article/details/gbqxnmcdb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gxcvercvt.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/ggywyrigc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gwpdpleen.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gzguwhjnv.sHtML


<!-- 参考信息 -->