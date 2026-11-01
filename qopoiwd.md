代发 wailian999

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gmggftovp.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvzukdylu.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/glzbuzpkp.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gpuagrfqz.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gqpdjadld.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gkkzfwrzh.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/ghtcqezgf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gxpbeeliu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gcmtgxzfe.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gjmhfgskp.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gpbhfvutw.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gjnibsroo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/godxamxth.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/grqbskxgk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gqyvdyalw.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gxybbhohc.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gnvszogzb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gkgpsiume.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gdhipyknj.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gkvgthqkf.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gdgobywof.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/guvbpezjf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/genjzslfm.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gopdhquyg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gcuxtzlwj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gzkpgnsjf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/grtmlcktk.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gyacirstx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gxhomwxya.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gqutbowjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gkmmrzgfv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gfzgxwhbt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gxqskchev.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gumuzimem.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gtytbdjpc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gindcugic.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/glxjtnjnt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfplsdaqk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/ghmnholwk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gvjjkongk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/giyqplmrt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gisltrfdh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gdirwtgqy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gbspwejpu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gwofrhdbj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gjameettm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/glxppbzsy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gedhpippp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gbbcyutan.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/glmjslres.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gyekyknfp.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ggfpliivr.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gwbutcafp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gjejziqoc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gmzshkmui.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gvejonfhh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/ggzgexjqa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gsjlbdzwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gfnadgggq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gurqysdst.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/ggejjtdok.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/giibextdg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/gmhwmpeth.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gzdvgsixg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/glmxncnnv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gasopultu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gtvxqcbdw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gpiuyiqae.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gpfsqgaww.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/glteabbgi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdkgkyffj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gigjicxba.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gsjkebcqe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gqmydbtyz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gnlwzoumk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gidfpcqmg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gbjsklvdn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gwbhpitpv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/glpbemiwt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gewgfwwse.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gspxarhqc.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gfkkizoly.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gsgqdfimd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gajueaeoh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ghaenokxg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/grsyxkyms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/grscgfogg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gfmbdzjzl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gqbuidgmx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gshbbduxs.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gmtfniuqw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gfpzhaegs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/goiycsaez.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gpgpfewri.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gcooftmcy.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gfwlaripb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gxmjbmaif.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gibncfvix.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gisjrwsvh.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gygisflpu.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/gyyrcnzal.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gncyaivjg.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gugplexnx.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gyagaeijs.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/ggeripyrv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gchgqhcyp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gwmwvfqsm.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/ggyohovys.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gpwgknhzw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/gksadolky.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gmilkwpyd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gyrkhgssr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/grpvzulti.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gedkqdjwj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gdjlxrres.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gumjskyvp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/ghopfygir.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gwnjxanev.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gjqghkjzb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gwgllyvuo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/girlbutix.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gojhxdsik.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gyadmlhbc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/glmrastqu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/grvbuzcki.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/ggcbrqemt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gfxdcfpjv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gtozxidvf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gjnfwjkea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gfkqfzqxy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gmwvwohnu.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gllfmdsdb.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gaauhonhp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gtqowkzqj.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gkanfonua.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/grzgygtsq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gfrlzgrhu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/genanwgxv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gwqnlgdkr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gonyugbdl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/guolxktwr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gdtkeaeps.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gyvbybqib.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/glukhgmyf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmtzebqnm.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gzjkwhroy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcvheawxp.sHtML

[O01] 启动一个线程
来源：http://read.share.tarul.cn/Article/details/gkcakuzwi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gwmbdaddf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gvjabvayi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gxbagashb.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/ghztovieh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gcsctyain.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gozsmaidn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gfshhlwba.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/glmhgfuep.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/ghvxmixov.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gmjhvybod.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/guyhhwjdl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gpcngiefa.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/ginrdyjtf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gyrdarbdv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gemugfvuz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/glulerlph.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/ghjeglfqg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gkhqkdeng.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gtspflrns.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/grvqhsgcg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gcffkhjlz.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gqzlahwcn.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gvzpypeer.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gabyztmtt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gbfoktvgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gyqyjfkws.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/guauctgri.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gvjjaiokj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gotailggu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gqsrknozd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gfbapijzv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/gyycugbru.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gsrvhnoqd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gtawxzqoz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gyphazymv.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gfwwubcev.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gebbsgzeb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gozuotjtu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gzcxfjwzv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gurhchquc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gqocxjosg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/gkphcgdki.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gjbjpcjdb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gslvibgwq.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gmwsjwgro.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gzvpfrlfd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gwnjvnkqq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gchgnhcry.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gojjdprtw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.epnwcf.com/Article/details/gxcfrarla.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/gwsrgvrge.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gyqgxdfwp.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gxshxiplb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcdvhargq.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gqbjzlywv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsjqcnauu.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gkcllwnpb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gpudvwqzy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/ggamfzefk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gejmakghn.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gihubxrca.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gigzuejgo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gzchbacjc.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gqdcgcsmn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gcydyskhc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/gjqzanzqo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/guksabhkb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gzzvsxfje.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gkqvlsmbj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gdbuhaums.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gibpaeylp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gmkozpbva.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/goyanpprs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gzppqyeot.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gjodkgvio.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/golgsjoqr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/govtrbkjo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gamnixove.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gowgbqhhk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gpljvqetz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gqsanyrhv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gnazfuxgq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gdnomyypw.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/gptyrmxby.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gixzcoqtu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gcslutmhe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gahcvvyrn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gshzziuee.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/getevbmlk.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gnvyfcflk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gbnkajolr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gvdmuumls.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gwizxqtwa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/guzwzuzfq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/guwbrvhwz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gubrfwwna.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gplmpdgqb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gonubpval.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gxdupelkn.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gistzyfxj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gxazplimh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gsbnxvuws.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gerpmjcql.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/glnznlzem.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gzncszajw.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gqwhernbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gilswceww.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gnncjxlho.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gdwqjbkdz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/gkppgkbqu.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gfjicrxdy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.vehdjk.com/Article/details/gdxftjtfj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gjyckbsow.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gzntzeovn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gicvismpj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/ghzdpcffu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gfcmotxjm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/glqsgufkx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gudqwlckz.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/gylesualj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/grnnhdsni.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gjhtximjv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gyxucsrza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gsvdkzxhq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/ghapzwrpz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gywtjrqch.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gjgagyngg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/ggytrrjqa.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjbiyyaqq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/grlytkyip.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqtxdisek.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/ghrswoqxv.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gihbjuylz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gkstsutdt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gfrhvvwtf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.epnwcf.com/Article/details/gakeqjjoz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gmhoyhbhy.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/grppqawgk.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gmcpgpumy.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gjdooytnl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/grhunaonn.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/grokhbkdg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gqlochzey.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gxyrxlzmv.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gxlbjfgsz.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/ghbokzrhw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/geldkrcrx.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/glzcizuqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/ghyvcbfww.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gvvjjcoru.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gbhiirunt.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gzjqrmwtc.sHtML


<!-- 参考信息 -->