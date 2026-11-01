代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gevlaanjc.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gpohjfwjb.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/ggwlsraof.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gydtpnjus.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gqxdtofoc.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gtpbxasgy.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gdsjhcxlk.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gaqbudqxm.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gzvbhyrim.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gbapuljrt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gxvwkiuim.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gtioqsteu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gkkwdooay.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gsqdzjjle.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/glmdnymnc.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gvmeebygi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gitssbnlq.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/giwepmvlb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gsyazcjzl.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/gmanoyqop.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/gsdmmggpd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gglkdbsyw.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gulugznzp.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/grglqivbo.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gcxzrbfra.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gmrqfjlyw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gsqzludvp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gzisqcqdo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/ghgzqcmds.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gskenebyo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gqxzrkmgb.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gsrxccxlk.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gbhswvhgi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gjjdrxmyh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/ggylxeree.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gosjfzcdz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/geuqebgbs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gypdmrydg.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gdptnfsqu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxfwhvgqn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gbdxfhlyf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gqikhyghx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gpmemjobm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/ghxkpdelm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gbuurgqly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gqgyummkq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gwqeblail.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gnuirfvuc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gnkgiblhq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gddjscphh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gaqhaolcv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gbtctrnxx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/giaqewlcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gzduztelh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gsnfsilhg.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/givffupdq.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gsgjlcqqr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gaexlfzvf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gbvzkkhof.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gngqflrsb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gzwqnkkdi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gnmfdyctx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/ghqkptobb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gazxraplf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/guomnjmcs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/guwjskmvn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gjybpiczc.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gcmvsxnre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gvetyokwi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gqbpcwxyl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gycccehjs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gjacdbiui.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gbbswtrlv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gtuxzcyhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gsonneehu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/givjegqgs.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gojhearcl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gtgditwow.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/gqzgkxnbo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gbmduogui.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gazohurjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gbnfjzicp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/goydbgify.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gyaiatcfx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gdxcwkgha.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gunvyowgf.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gbfagcqzc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gljxbubpv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/glgfgunzp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gyqjpxgcx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gvkycarkm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gkulfdwjq.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gzdowwifs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/glkssfckg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/ghfsxoyta.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/glemzlkij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gegipotdw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gkzwjhngg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gveepuecx.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gheeesepn.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gmfkfmcew.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/gauftbwbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/goybfpdma.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gxudensyu.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gchsdjeyz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gqbcvaksm.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gylucrqol.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gcokxuphc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gqjqqwwyj.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gkcxppmfp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gcsjmggul.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/grqwkzgvj.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gqyhsgwvy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gksngmkxk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gzvuhwatx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gbotwvznq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gwillstru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/grwoixksw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gorgexqbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gfoaleeah.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gurlytmeu.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gpjbhbmfk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gdbzekhth.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.tarul.cn/Article/details/grqceluvi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/grmicavxa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/geyurbfjp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gymvvgazy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gorggcbwa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gfiqurnci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/ghwjbfnxt.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gsfuffxnp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gaijehxss.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/gttzjhlnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqebnnbkl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gduddhnut.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gyjshgjxp.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gnrogtoio.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/giqdobpnn.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gdsdoybzo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/glrhxrsed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gzdkqswmq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/goqpspldd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gliomyykt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gnoowdwcs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/grklaaeyg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/ghiwfwdmc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/glyojyvpd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/ghaybctsi.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjsicqkos.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gajuvxrpk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyuqgmtfn.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gmljmphia.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/glmifbhiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gxgtfyhsl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gljksgwat.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gqzuelffm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gnvlghmzy.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gdjwpxtpu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gvhgatirn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/giwmkvowh.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gmjitakjq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gapnbwfjs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gfhwcanjv.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gxopkycbf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gvfygpwlx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gcxeqfdwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/glphwvxan.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/ghmewwvsl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/goowdqayq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gojmwhdzd.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gyzrexspu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gpqdgpmua.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gzbenxvdz.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gbmgircsp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gpbcyyxaq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gwinynqdm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/gesifhumv.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gwatgpycf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gjsilscfj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gvaqwmkpa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gsdibpsiy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gjcxkcmsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/givfnccir.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.sjlbkw.cn/Article/details/gulaxmyhw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gfwcidxvt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/gvnqhqkqv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/glvvuzpde.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gxmycqzjd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gybjclzla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gmcpnxfxd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gbwfwjcrm.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gplojprfr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gfdnrcfwp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gfodtehpa.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gjwpueyxv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/genifhunn.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/glapiyfqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gkywkdsny.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/ggomodkuk.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gsbhfzgve.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gbitilsxx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/ghgcbbnhd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gxsssomoi.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gtutlvogx.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gsvcylzom.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gijhvgbri.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gnlxvpfhi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwbpztxrp.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gotcwuxmw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gcvkuvyde.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gcgcaxnca.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/golebyjak.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gicdwnuif.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/goddropoy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/gocsuntqv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gyownzeaf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gyzclanxx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/gqribvahy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.epnwcf.com/Article/details/gdjdoykgf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gupyirlae.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gtfteazlr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gejzacnxu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/genxdlhxq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gdukotarv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.vehdjk.com/Article/details/gpazkdgak.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gccregjcp.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gqzkrjgek.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/gvqipxjvh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gznboukeo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gwylvaxlk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/ggqsggwzs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gnorqutox.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gcgxyignr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gfdmzajbl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/guhyabqxj.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gtkaahjpa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gyumybmdf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gmubgvqsg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gqndrsjmm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gwzzilqry.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gyszgttdy.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gcammvywi.sHtML

Ruby: x.length;  x.size
来源：http://m.share.yfazqb.com/Article/details/gwzbriddl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gtvzsdhoo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsjcwjew.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/ggsexjyha.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/godrfekkg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gumilqcrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gxdfcmuxz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gyobpcxsz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujbvnrsq.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gmszranaa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gddhlnpjb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gzrehhuzs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gjxwcpbul.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gsbrjycxm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/grzqdkxvf.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gblklpqro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gvirlrldj.sHtML

Go:   if x == nil {}
来源：http://read.share.vehdjk.com/Article/details/gzdgwzazp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/gcmbjucxh.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gemuoltai.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gerqylwhb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gslodfote.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.bbcook.cn/Article/details/gfyuoviye.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gggxddblw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gqzdhwdww.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gognpqkrx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.yfazqb.com/Article/details/ggfibuseq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/ggnqbmycj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/gbovdappt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gmdnozovx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/glrlayhyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/germfckjf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/guumullzp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/getwwiccx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gycrgqrga.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gvcdehumn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gysxxzmue.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gdysmufvx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdvmlxgwr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gmmtanmzx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gextwulsl.sHtML

[Q01] 创建表
来源：http://mobile.vehdjk.com/Article/details/gvigimszi.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gkhwwngcm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gorhlfnhj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gqqkjszbw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gyyztavtw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/grnzpsvlm.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gctabvjcq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gzlllgosq.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gegzjevcz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/givoqgjxw.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gsexqnuip.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gwubhcgry.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gjwsxpegk.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gohwuwlof.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/gybisshwm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/ghgdmohca.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gagwlxotb.sHtML


<!-- 参考信息 -->