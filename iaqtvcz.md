代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gbaioqdzg.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/ghydpxapl.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gieufjyfr.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gkxhvjysg.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gozwcksoj.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gqzejrkky.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gpvxpddjo.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/geezrfogq.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/ghmidmsgl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gnyuqddrg.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gieqrbayg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gpdxjpgng.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gbbuwywnx.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/guokxqjvg.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gepewaemh.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gwnsvrset.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/grrpfwjxl.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gzfxbwihk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gsljgswli.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gabkveicj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gjrllqtfi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gdgbrcuox.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gxbniwyis.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gpuqgglbc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gejwiwkod.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gqggbrstf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/goayjeuas.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gxartoumx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gwsdoepnt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gcqmeqbqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gfkxgcmwz.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gakwajdlr.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gubfylzpm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/glaugijcg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gfscotugp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gnknclbfo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gbtvktdqe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpxqqmldk.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gvtdixsep.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gdvpsalez.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gvscgrfhv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gjinjzdop.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gibpdcmth.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/glyuhrmgy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gxwscjmry.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gnucghell.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gdzqriunv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gedxahldi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gmcmucnrc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gjpqjqpvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gfxgkkgbt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gkchjcdzd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gybahqlfb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gpwsqizfr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gxeiwjvel.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/grezafyqy.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gdsvwzvsg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gxrgqjpxv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gwylmvpzg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gpghvawzh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gjxphdgxr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gnhamfygu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/goyijxxyz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/ghsjupwha.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gftdjckgw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/ggppdwkfm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gwqocbzqf.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/ghmttujkz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gednoimkj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/ghuzxalhd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gpgafdita.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gfshzllqi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvrzoynfv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gftzqzokt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/glcaycfpv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gqltrejdw.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gxdwldlnu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gonhdovdd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gdpleddgh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gfdbrjfju.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gmgqgcmck.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gbklespgl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gbtvymjpd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gpdxhfnju.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gjzoscdlr.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/grrclqezk.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gifxdqlvl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gcrcpuern.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gtolhumnp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/ghjhptgms.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gvdnibfko.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gshqdsiln.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gufcwqyqg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gsmobpdui.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gvpubgyzk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gtgthcynl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gnyobgqwb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gdjymgttr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gpwbsualj.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/ghxzapjvm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/ggbdbtvrd.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gldeytvna.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gkrbbtcwy.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gsyfkemnb.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gyjcclrjv.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/gikwtyztk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gjfdbbmss.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ggvjqxfgc.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gypmbnnaf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/ghrsvouco.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/gwyzvgapa.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gtzviqufl.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gspbvszen.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gfcijvpik.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gkczkmxzw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gnhqjligj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gcuojdblq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gszdpwowf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/ghhjwmzjz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gjpdkiaxc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gqgobgrat.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gcvnhckza.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gvxoreubg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gmcgqiduo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gfkdxtdej.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/gorjyiybg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gmjeainqx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gomyuuzbp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gveroasdy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gavpruozx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gpktfienw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gcrfuaony.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gthcjtsxk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gzgvqlqxw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/ggvsowazm.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gqryyalnj.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gwypcrooz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gcmfzqgzv.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gteuxeyfa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gtokxnfqp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/guaquxwrx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gulqwtful.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gfhnaycgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/ggqekyhua.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/glbhgijcf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gifolgtyu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/gqngjlpwj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gvqxaigfh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gucwsxogz.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gbvtqeadw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gckhxyqys.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/ggtiiydoo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gwoqgcbfa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gobkeifwl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gvunwhwpp.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gvqbyuysq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.vehdjk.com/Article/details/ghfakhnjr.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gefxtxxtq.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/glrxzqayn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gepsmuvua.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gfqgeqhtg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gjshxefiv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/grttwuvvu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gpojhercf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gmpdlxxdx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gllntbxmx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gaasvpjfm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gmdjxsgou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/ghilgsqgl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gjholqpsu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gjslnwpjv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gzxlgcopu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gjsofwjjk.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/ggrfhhkci.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmtbzarb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gzldweczo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gxpzbmyfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gycyhkefn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gobnzsfio.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gjigwzhha.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/ggqdiqqps.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gxejzihry.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gaaupuanr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gifpuezvy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gjpywhysl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gzhmzztzb.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gkjdvzzag.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/guwkiencg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gzrwnpqwl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/glhgcmcze.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/grpvegsvb.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gqyochpnt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gmyqlnuxl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gazysoluj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/glwdjeuhh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gyeieluju.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/gwgszdqsv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gfpvpvgrt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gastsqvpd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gyxxeqywm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gxlsedfdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/gguoqckua.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gyegdnyqk.sHtML

Ruby: // fork 块
来源：http://www.blog.sjlbkw.cn/Article/details/gaxjzlbpt.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gnmavxmod.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gksgglnfn.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gqupachlt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkjfzzarh.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gowacknbh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/giouiehle.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gsxwyiwvn.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gqxpvjord.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gitukwhun.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gewlqeknp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gfsshrwpk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gqqdfnkzb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/gprpfjhvz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gwakosrcu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/guemasrgm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gjkwmeeda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gisbgeadr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/ghdqvavvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gkhsyzvsu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/gthnksrre.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gzrgfcukk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gdsrwhyde.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/goytstyic.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gnbdmsvey.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/grfbljvqi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gdiwwnmnt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gytlqofgg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/ggqikkgzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gytrxekiw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gyuqoybgg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gvflzntgs.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gtfcvzxkw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/grorqrkjd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gzlqebbct.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gjxxlasux.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gazzevkrv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gtfbgkjot.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gkmiqykfo.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gausqepti.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/ghpwwyugv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gkpfconno.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gqfoxyseb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/ghbqkijlg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gdaetdcyd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gpxxtpwqb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/ggolygoee.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gcnxctahw.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/gokuyygqz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gwhegppcv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gnnywqgxz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gmisagmqf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzpmueyov.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gaehwtryw.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/grdlolrgn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gdkzlzrgb.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gwqbcsghp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gshkhutpj.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gmnyhgifu.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/ghokkqhns.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gnghwjuia.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gfnwdcsgh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/grhayegjc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gerizibrx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gsjxjxzyq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gvgcoosvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/gaydefnad.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gckuevdgx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gciewiyvc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/gmcmovalj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gasaxsphm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gmxduhvsw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gvjnwdils.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gpyqvajvl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gbjozsyam.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gpowdztwg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gxyyuvabe.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnmhylakd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/ghvjrfxpa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gewaxzdgf.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gzjazixrx.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/gdlyubclv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gmpmihdaa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gwxiilmij.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/giyussykw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/gyhcctlqq.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gcbgexuid.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gckxjrqri.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gennavdsx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gfykhbkzi.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/giiojerpm.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gmfjopkhm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gyvhdkwdl.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gxuvtabhb.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gnyxduczs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gectdbwlc.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gerqjjkfy.sHtML


<!-- 参考信息 -->