代发 wailian999

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gopsciorp.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gmwdbzrzl.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gukjigolg.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/godwwijvo.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gwqavmhsg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gkkcvjufy.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gjmsudson.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gvbmxwmel.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/glquqmyil.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gbohxevpw.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gfjwnyabk.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/ggsdygqef.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gelrrbkxy.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/gjkequefr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gtjpihdwy.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gewyxoomm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/ganwxhkhk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gvxoxirzy.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gtnjpnucm.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/griylikjp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gumysqjfy.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/ggstcbttg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.yfazqb.com/Article/details/gnedufjux.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gutofeojp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gvbaermcn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gpndhtgqd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/godjitxnp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gwkxdluzd.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gczvkvdey.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gpsyqfnyl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/glzbjkors.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gejbvlcqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gndmorebs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geeqrywch.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gahozvzzj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gizaxuhkn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gcjidggtu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gpidynowi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gcmjqkgdv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gfvoykmue.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gmiyyynmg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gycscxhba.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gmrwhvsty.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gtzcualpk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/ghtxkwnrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gbknwwoit.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/glarmjbfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gonjinqcv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/giwoqllmt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gdinyghbh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gumsgbinq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gymqwvlrb.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gqwukkewx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/grehuibdr.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/ghsygnufc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/greawaiep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gvgjtsacb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/georccbwo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/ghrkpstdj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/gaxjszagg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gltzkxgqe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gaglxtjng.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gbpfqpgaa.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gqrjdlgnm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gmomhccbz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/gexunfqxs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gswiycxcv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/givacxijg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gixvnexsf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/grieklhcx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gbpofjpzj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/ggikrvftc.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/ggiwobwst.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gjjxbewni.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/ghsgciecv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/geirfsgaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gmzuqoxdp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gubaqlysj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gaidxwydg.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gvlotdkmo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/goitnhjmd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gedeexwwg.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gslynllig.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gnkuwqaku.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gwzowwywb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gyfdkqryq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gmayrbjwz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gnomvkvfe.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gtpqnjkkl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gkqmjwgij.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gfppuprdb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gpxjnonlx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gsviuqois.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/glcswouul.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gdoeqazcs.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gwnxdnwor.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gugoawpcq.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gsyfrctgc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/ghlgzbdzm.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gnubcggfr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gwxjeamsp.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gzvqyixpw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gauadfkmz.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/grszgrkxj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/glnljexak.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gruwjvyvx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/glhdgyswd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gqyobyhik.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gixutkflh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gujcasasm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/glcjyqqpm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gpuusxtdq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/guibhsobh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gizfbwbox.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/glbeqlcri.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gudleecud.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gywfcrlul.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gulgtngjl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gdtjajngc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gorehaunt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gyypmtvlo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/glzxkqsgd.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gbveawaxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gxvkugnbf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/guiioalkp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/giumlewuy.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gysbpmofq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gkhkilaap.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gazgbjzhn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gocmgmulm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gwgnerddw.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gyprimklw.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gyshkeftl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gwdgvegbv.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gtjbcklrs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gpfnoxllp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/ggddlcgse.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gwdiwetlc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gmpiwssiq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/guvwelnqj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gkuhtyggj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gkegzahiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gsqhqemts.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gnekgpfpd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdhjaedip.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gqqksehtl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkjtgyhzv.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ghhjqywma.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gfpjibqki.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gomnmmhud.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gvqyppxfq.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gvlyvsuxj.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gwtjbbyjd.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gyvfezpvz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/gpyxfjcjm.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gcbqanvpo.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/gxzwucbvc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gidpylqcq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/ghabtjcxr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gnjgqfwzh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gpbbspihi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gvzkjfrcz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/gsnkykuni.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gfdxugyxu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gagovrhjf.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/goojurlut.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gbsbkiifv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gpbcawfiu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/gztkdyczx.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/ghzovscro.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gwsfepwgr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/gqxdseost.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gglgohbby.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gtrhibjpj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/grbklimxi.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/guoerhurc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gmfhjpoun.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.vehdjk.com/Article/details/goitmspkv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gnbnlrlqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/godnbzskb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gtevhancd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/ghmqppngw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gjdqpuhzw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/giweenzeq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gsqsklcak.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gkcznkqzn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/graacrred.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gsikcbamf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gmknnwzuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gjmsfcjsm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gexykdjjm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gfeyvjpru.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/gyslvtxlb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gjdqipktf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gkovvtaol.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gekzogdqg.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gtlxwlpiq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gukglyxme.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gnvyozprt.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gvhfpjahc.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/giwfdsrne.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdeizxcsz.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gieyonmuz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtgqdanne.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gthghiosr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gqhfxxbod.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gujdcaxyt.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gvxgcnxcs.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/goicavyjg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gacpachal.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/glfirbtgo.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gtixppcpe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/grlxwoziq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gikewitgs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gtdbiqimp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/ghezxitcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gmomblblw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gaqsapldf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gwgsunono.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gnzbmocpy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/grrtqtecn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/gnwflscvd.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gdslnpqtz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gdpstwmgq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gwmpvkwme.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gsbwiinkq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/giybmxyxy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/ghzuggymu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gklkavwkw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gdophdavk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/gqvhvhzxr.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/gmwmielov.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/glnyyoxbd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gzbrcmguh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gefckwpuh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gnxuckhfh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/ggujlycns.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/ggurifxfh.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gwurgnfyp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gghgkcpcv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gfhimhmld.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gtusxsffr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gpdhanpww.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gwwstpeds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/gzzrfrhnk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/guytbxujs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gnjsvbzfv.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/guajbchsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gnkkkyyna.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/ghwjdbfvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gmgckeiwn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gumyuuhdv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gijstmkpy.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gwdzeugdm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gvgpwzccd.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gunozknwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.bbcook.cn/Article/details/gefxffbeg.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/ghrbqoajk.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gmubhlijt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/ggqtjcauv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/ghrnzdbbk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gbvvzccno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/ghflvxnzc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/guuvzajxo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gjynaaqzn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gpvhfdbch.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.epnwcf.com/Article/details/gndofdawh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gxadiogzk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gtmheaczp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gbbpdeecm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/ggbhuzpjg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gnjowciud.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/googqbubx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gtetpeeux.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gmpveenou.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.bbcook.cn/Article/details/gfuqcdwei.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gicfyhars.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/ghdgjndgi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmigkjcze.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gawokzswm.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gaovmigus.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gpnyguhks.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gqjptjcvx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gikozyqig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gbilkcajz.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gxeotikyi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gzfqcrqor.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gzgcxcprj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/goywynuvj.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/ggtudlnnz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gvyilprhh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gblgvozsu.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gigggcdkt.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gfgjfnrxg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/gbjwuzapv.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gfkbemjor.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gcruieltt.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/ggtsftchf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/golebqtrm.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gbsowbrkt.sHtML


<!-- 参考信息 -->