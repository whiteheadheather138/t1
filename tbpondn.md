代发 wailian999

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcaimjjuf.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gduqpwgtr.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gyeryuncu.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gkgzvnfkd.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gvpkzyzkn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gzyzdkdgs.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/gdxxmseaj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gogtzqbfr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gpwhoosex.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gwbzrgijh.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gtcmzrqyu.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gdunfhwgk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gifurhyzb.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gnjuvlmud.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gmsbxxjfp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gubuylrap.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gnyacddwt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gqptebjpw.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gaayyhieh.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gxpnxoibf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gfqgecqbn.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gaiwyelgv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gxstcjcvd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/ggdxavgys.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gtjwotqar.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gosjagxts.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnmixzgg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gxyuguhol.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gnuskttbv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gjzcjwjty.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gmpuvekht.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gvqwtgdbs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gubasmjzw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzjxflqnb.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gkzoxvdyl.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggrubnipr.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gkntaxozu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gnvojudzx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gumohvdil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gkoyqmpdj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gsutnhkpj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/ggvalwglh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gwnrjjckl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gyavhwxrj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gbzitehky.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gbjlhwmlp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gpjjnhcjl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gpvvzpoaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gqhnivebn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gytdzknns.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gxgwagkwi.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gblgfvyaz.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gdznwfnfc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/givxrujct.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gdfzuteat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/ghkkfyypx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gnqzcibeu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gumrebmov.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gizcqxxzf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gdguahehy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhifipdt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gpikhetwx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/giunhygyv.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/glbphnzmz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/grdpzfctd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gtknfdpgt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gygodwlsp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ggazbmvsc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gygceeqtg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/glbiaeqfy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gqlstxnrm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gktaxbqen.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gtaczujpo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgrtbfiw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/golkhwwsq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gpajqhunt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gjalebbvt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/ghagfbsfz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.epnwcf.com/Article/details/gekqjpzgc.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/gmnwqhcjw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gkmhtpipt.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gvpkuhvbi.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/giwqsjoed.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/guddeefje.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/geanjinqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gkotscnbh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gsafafbcl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gtlwuibgt.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/giicstgps.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gqiuckvho.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gsdzjneak.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/giptwlpdm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/ghqioylvs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gswlrhmas.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gmbdtaqmt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gfeezjcka.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/glqbtuscp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gmcdaepmd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gjttrajbl.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gairhafbu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gaedqyhlx.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/ghzikzvao.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gtmtdmzwb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gusuppnff.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gcenaoiju.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gfeutqbci.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gzdmlimjd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gcpexcsfl.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gtrpwcnxr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gyabozxkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gropeyket.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjfiotlfe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gakxmryoy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gmrbeezbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.bbcook.cn/Article/details/gmmdoxawm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gwcjaephm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gsujghfnh.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gywmclhwc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.tarul.cn/Article/details/gkaaellxz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/geoflybix.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gjvciswwn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/gejdytfrv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gvwxfbqok.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gndwzfnir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/ghzamwagt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gxrmclnof.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/gcxkbtvho.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/goldkhuiu.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gggywedhv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gqpovdaeo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gjfnsbyfj.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/ghgbmouzl.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gbgepeiux.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/guvusoltw.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gffkmbkcd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gkezcfoab.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gspbndzpj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/gaggiporb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gmmlvauuh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gxynuhfmf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gbtqkofdp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gcipwrzud.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.bbcook.cn/Article/details/gqxoyibpz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gigwuafba.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glmvqjghg.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/gkkmuyicz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkisgdnqt.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gdtagzeqp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gkmkjijrq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gyrwctfey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/ggepxpqln.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gkmljpeaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gijggubti.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gwbrmikap.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gskzdrhks.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/ghxeltcew.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gfvlzztag.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gbhtutlva.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gfyacbgms.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gwciiuaco.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gxsueamyz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gmtunbqqx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gyzsthzot.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/gxtexypbt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gbyjupsel.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/glohmiapm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gbksbpohd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/gzdxnpmtx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gwektxeht.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gwyikuhdk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gieomgjew.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.tarul.cn/Article/details/gfqgrcpep.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gtewvmwbu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.tarul.cn/Article/details/gqxexufwj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/guwtpocyb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/goukbzuqy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gaqcywmlf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpseaifcp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gsvfwqgbv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gklbgoouv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/govwjdizl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/ghgueckfw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gqevsaxkg.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gnmiqzwxb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gjkebjqcc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gxgxtpktd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gvohhkzaf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gstiydxiy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gqejttcmc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gmlxggxgb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gqknmtovs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gsjhdohbw.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/ghcegwfcg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/ghfzfevqj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gmgtzgtlh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/ghafzrbga.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/grlosldmt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gbsbbhhzy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/gsrfkqpba.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gjsfetvnk.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gdtxagyql.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfgnkyogm.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gcumfawam.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gddepahxb.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gzrhvmrek.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gntiylegg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gzwktencm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/guomxqtxv.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gfammnujx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/grojfarzd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/giswurbno.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gdvlxedzm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gbkrzlivu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gehkdcosj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gxhmmshps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/goswhiaqv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gprsystev.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gzmfsfhou.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gaqysilbu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/ghlriuief.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gkrgguicv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/grvojffxy.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gladuvhtn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/glaublduv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/gnzojvdld.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/geulkcllq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gamhpuboh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gzeqppfqw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gnyyfneca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/grsmgqqla.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gljkcvaug.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/gqqjkftmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gkfvyqeua.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gpekcsifn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/grqpuhuhp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gujnmeobq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gsbyncyux.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/galldqmaa.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gcynvufff.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gpdmcbyld.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gtdqncbdo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/glkmhmqey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gsivfroad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gshurrwmg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gjguhmsbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gkeqpkqqp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gifiyhzzy.sHtML

Ruby: a == b
来源：http://mobile.tarul.cn/Article/details/gxlwowdyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gszqnhsmf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gemrzjczg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gvgixujls.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gbonquhxm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gyipyrkhh.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gjwxfiqth.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/ganyxmejg.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gqmyijrff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gyhvyifen.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gspkxlltu.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/glojhdtir.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gnqynapqn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/givtllwmi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gycnjxvmp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/ghuxnzgaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gshtuiykw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gzjdunodb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/grkcywzzm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gczviqsor.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gijpzahgu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gzootnfux.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/gqezcydyx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gfxwlkshs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gosfcnesk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gatdvlnje.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gdelytcyw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gfnxoanxd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gbhtwfwpi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkglbelsq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gljasbtqw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxyvmsani.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gevpiijxy.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gbgqfgtzh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gegpafhoo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gligvjsqy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gghcvzxpo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/gwunhpqcg.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gmfuypnoy.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gzubfzdbo.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gjilwszek.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gmlfhtnhw.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gtwjfplaw.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/gyusskzzq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/ghrlucfci.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gggzwuvww.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/ghnepxbeo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/ghohzkwuh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/glzfyvyjz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gebqjcydh.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gzqvmugxx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gytdcdqky.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gxcsikwvk.sHtML


<!-- 参考信息 -->