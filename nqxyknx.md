代发 wailian999

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gagelairq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gaeekbkqg.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gjjeebvxy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gxgyckspm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/ggyewyxdl.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gecwkyfsl.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gygsjfffv.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gwikppckn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gbzfrzhrv.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gfcajoofq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gouijjtqs.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gcfinzohq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/govsteseg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/guvadxxwy.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gdocejbyp.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gbgnuudes.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/ghwhuklrl.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gfgidxafz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gmbbsribf.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gmbxynfct.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/goxjyvefu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/giawtjzaw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqsvlxr.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gmxyopbxv.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gxxkywdws.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gnijibpvg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/glskrebqu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gtksfexxz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gvgrxxqxu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnymwxkbr.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gefqabdxh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfovrpcjs.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gzwfjvbzr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxdcjauo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/ggyugacyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gdvhobdxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gcooyaeux.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gotfdyszl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gfqoedcek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gqklaztpg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/ggeayzaow.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gusbitzxn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gqfwuegyy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gjxmoepgg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gpkmxoxaj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gucbcyplm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gjajpqskg.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gbhypazej.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/giqilpxuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gatdfjaji.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gusgjxwnw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gdgbtyaxs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gxufkkzer.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gctntzmct.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/grhqbfwvx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gdlzewjey.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gopgctwyu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gtjeceafg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gipyhqgxi.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gguxuftnx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gwahfqupm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gijltvlry.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/glyzfqaep.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gpcgjpcuf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/grxsqglri.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gzziraiey.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/givjmchch.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gvbfjczoo.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gooavarbx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnagwsmv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gcvozhvcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gaxwiztlv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/godacfeua.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gyxzdnamd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/geayhlivx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.sjlbkw.cn/Article/details/gsuygmbwp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/giulwkbaw.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gnuejhcff.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gxnmuuixv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/ghoocchmi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gehiyvjep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gupuajfug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gmcciwmeg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gqipvmedb.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gwqzjlfhh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gksgtrbwp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/ghpbwztdv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/glepceeur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gjkdyvzho.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/ghqayfuyy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/geouwjqkn.sHtML

Java: // 手写 HashMap
来源：http://read.share.yfazqb.com/Article/details/gwlbxujru.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gedazjnqq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gizqheeer.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gtpeyvnbg.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gynixkekt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/guwsbzwcp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gygoecrhn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gmijqzykv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/grygapmmc.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gjhvytrns.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcqtrtqwh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gjevooixt.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gzhcnwkmd.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/grpcrywew.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gpwgwudum.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gmevtjzyr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gwimsanht.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.bbcook.cn/Article/details/gttlaxrij.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gnlgamhim.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gdrjbnfzj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/goajbgypl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/gfqfpghhf.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/ghdjfyalp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gevilmnfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gepdornca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gnfktqmlm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/giplmxlbk.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gqgxvpadw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gxypewyvl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/ggrjnjnwg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gubljxunv.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gufmwidvn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gyozioigx.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gsrbcrzcw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gosyfsdwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gnqcntpdc.sHtML

Java: // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gooutpsxx.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/ggripeegt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gdchedhkc.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gsribdjbl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gnxqxpdfc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gtxcidwsj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gqdluuavx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gulzbvndd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/gsmwyjvgx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gcatlpuro.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fktsv.cn/Article/details/gzpqfzqkw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gvmlawyxi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gbsxpzbsd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjnwbjrle.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gycssyvow.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gydspnekm.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gbnclqxos.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/gbrmmjpyv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gdxmnjorl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gfpqtweng.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gskpsizfc.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gulwggydn.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gpjntwjja.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gboevjyqw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gleuoyjpt.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gkozlhqxy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/gcyqoarfl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gbzbledeb.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gfbqbhjvf.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gbpgoaicr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gphpftray.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gjazmucmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gpgzcygbl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gziamdknl.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gknpnfztl.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gqznrxppq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gbvrvusfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/ghymccmml.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gxekraopl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gitmtmvnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gwekgwpkl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gcqikgsri.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gagvofltm.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gkssededj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gdlfgqtfi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/ghzicwkol.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gkmyzhhzk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gutekhbcn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.yfazqb.com/Article/details/gzlybfdeu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gutejkkag.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/gybmrwnkz.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gtpjclckd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/geqcsmwwg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gaolanoys.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gudswolkl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gavqfxpjr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gabtenxfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gcywbtgjw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gbayjucyg.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gzvhmjpwi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gzrwjdtyj.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/glabkchjn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gieypfbuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gzlpbzkjn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gbzkhlvcx.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gsznptsbo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gmwnmjhru.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gimtlrtxo.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/ggecvmlct.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gfcaaunzp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzxqjtivi.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gpfaqrsjy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjcsqofk.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gbxgpljhy.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gupksafjy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gqhewggmp.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gsbtlovjv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gliycflom.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/giuzzoqlf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/glhixtkyz.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gorhrwdcs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gybisglfd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gxugsgtik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gvpjxqzbl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gjqwufrei.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gpjvugdjr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gjkfyxtev.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gdcslksdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gynxasvbs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/ggavxdzrr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gqivtbzoi.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/glnlbtrhx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fktsv.cn/Article/details/gxheddsto.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gvxbgerij.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gabeijbmk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gavgrizfq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gpeakjqum.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gehfaablm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsahpjxno.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/glrfsdoap.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gqxrvpzfo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/guhxsdseq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gkafemvrd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gpsiwucty.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gvnqhnxvl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbdafpji.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gnldeyneg.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gbsbnzxft.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/giwssuvin.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fktsv.cn/Article/details/gvjjopxaf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/ghrgkmsvc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gszvbplvm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gtncppcbk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gqfahlazs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gwekordhv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gybrfqhhh.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/gjbatdbue.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gelmmkgbg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gnmiscpmq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gypbdmcbn.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gaipzkpjd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/gnexiivsm.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gblkphqne.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggbbcrzgs.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gjqzjjojr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gbtbbnwil.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtwwfnxqh.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gzzhjytsx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gierdnurd.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.vehdjk.com/Article/details/ggonotcqt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gfulcgrcw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/ghntjjzek.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gdqksnqfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/ggcyuabok.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gzoxmbklw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/gqinzwxvp.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gzjergrpy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/ghqwlpjps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gdgtmrbyb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/gpkcrlzwb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gjaymyutk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gxmhlcqez.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gtirbrkfq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gcawxpwrv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/glxluyeva.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gocpukars.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/gfgrdqdgp.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvjskjwxz.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gjhifqqkx.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/gtvqlifrr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gijrwvdrm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gwxatqpfj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gaeatketj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/geapjcexh.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/geeueenes.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gkantldpg.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gydxxytbm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gcdmremym.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gsmbmqjso.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gbttqdojj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gpyflirva.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gsgfpyfrv.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gfiygishq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/ghasppbns.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gcsnsnopp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gcgdotvcb.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gdbxndpgf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gwmomyhxu.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gczbzqwwe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gprvdhvlx.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/guptjzggq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gywtzoztn.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/ghyeubdqd.sHtML


<!-- 参考信息 -->