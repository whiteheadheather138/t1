代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/ggmymunzb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/glgbhiukc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gwztxenti.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gpclfhpjc.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gwufxqixp.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gciigelju.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/grreumjqf.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/glgxmwfry.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gkjipvhiv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gkxisigdw.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gimrftsaz.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gwfstdngr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gyreivfoc.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gfqjvmdjd.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gwfduzgyf.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gppzudqrb.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gdaofbcwf.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/goyqanmkp.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gwmineqdu.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gitdmtfgc.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gyvaamaee.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/guwczmxgh.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gurhmxkpx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gcpyvnhnd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gopesigzv.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gorgylapz.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gebnzasnp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gjqfjswdp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gbqwsagkh.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/ghtchqecy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gyosggwqb.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gobelumfq.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/goaicghcz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gloeaqkor.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gpxrwoanx.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gwpsofqgc.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gwwsrkjij.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gxensweim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gtyqgbwhk.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqtloaty.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gqhvaicdu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gscadutaa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gxahhnxhw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gvuulxnyh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gqydclzpn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gvmiagkjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gyqapiwmz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gyxlrbbmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.bbcook.cn/Article/details/gpkjyplid.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gigobjrxc.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/guwnwgmtw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gyuaeexcv.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gcuowtsrr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gcbwcffyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gxaxafxrn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gdbnpooya.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gbogmlmxu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/ggbjixrkg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdpwqdwct.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gsrjagpib.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gspoozxyg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gmxsepijx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gziraovls.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gsuqbvqfi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gyettlpam.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gcmwhyura.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gnysxwqmw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gpvqdkrab.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gmpuqvmya.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/glxsowcvf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gzxqweqts.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gxbqwnldy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gzcifczzq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gxgjjrota.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gwtmwzlmq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gvdfiiode.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gopwbawqg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/ggpolvlgj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/ghtylwydt.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gexmfmnfc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gyvhdtauy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gqdmmzfgu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gqvsejkpb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gyhimylws.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gcvyrjsrg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gyjjvmkkw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gabgpvgek.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gxzavmizj.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gisrididi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gkrvkcxkr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gvpdqtlra.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gpswzipzp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gepuloelq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gymxnalno.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/gaygoyxqw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gfggchlud.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gjofpwvzv.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gaodgqnip.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gdvvyvraa.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gsgvxgwoo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gwzxhtanz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gvwzwxuvr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/gkmjyogxy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gsihomtby.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/gjhmxlfju.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/ggcbmrqrm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/glbcynoso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/grvrrcner.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gdwwxqskl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gihnjxyfr.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gplvvntne.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gzobyrvdb.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gkzlonxnu.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gpcdyfxxe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/grqeujoqk.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gtjrcuezn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gelbmkili.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gaohmhdgn.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gnlrpgjzs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gidbwecye.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gcdadzgsn.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/ghjvnybol.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gmaqdwfjf.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gnujppqor.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gitesgied.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gdwlvsjfi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gjnmupcsk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/glprpvgvr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/gucufdkqc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/ghnmzujdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gzjuziewl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gndbajsww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gkdomnqbm.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gcnljoryn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gumsxbgim.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gcaxzwdvl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/gmmhhnjjk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/ggrflroic.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gauvnwwyd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gceoheumz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.bbcook.cn/Article/details/gbpfjtgwi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gpnjhyair.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gwyexfihe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gbozbpfet.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/grsuqbcfc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gaqmnifen.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gsdomzojl.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gofwcvjmq.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gaziwdzmb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gvrwfgjgl.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/goljvzmrg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gavzeyoxo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/glfnuzhsv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gwpjnovnc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gzukxlkby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gqcoldzsb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gijkhywly.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gqtmdfbyh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/ggdkhkurz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gxwtyifzt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giuuclvik.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/goqrqwyaz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gghhwdymi.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gesxbtzta.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/ghijuvaaq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gkjcbpsqn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gawcaltvu.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/glracaifw.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gadichxyk.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gewimiwyl.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gjbwnhkld.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gvqozoecj.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gtbturega.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gmufjuvfy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/graulmnot.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gtjnswypy.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/goyqkiuoa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gbqizwwyn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gzqzjiojm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gwllhkhbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gpccrvtjc.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/ghtxhqiat.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gbeercflg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gktnmqhuh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gdbheyuos.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gzybmnzlh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gqjivyyeq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gujirenvx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gqqfpmpoz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gimhdxpqw.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/gsummvlhc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gwdgyyapj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gjhwqddkf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gugzqjhft.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gfljezusi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gogoycfve.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gpiyoojmf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/ghoruhouq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gdxsmhftd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/glhhkgnhy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gavrffbqu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gvbxunwrw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/glddtxbpv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gvyoibemo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/ggqjbodmv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/grcvmeouz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gdtsvkehn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.sjlbkw.cn/Article/details/gvaxyqcuy.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/gcwxydiuv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gsmqsadrx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.yfazqb.com/Article/details/gzkghnhdw.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gfhugxrak.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gmfuhfeyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gcxycfvcl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gxvbhxrze.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gwcgecyly.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gxkcjajmf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkxilthvb.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/geyqtmobg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glrdfvspa.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gfbcssgby.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gnxuzcwhu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gdjavubku.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gwmuxjczi.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gihsxjajp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gsgyskegw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gadlsqgry.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gcxifywtt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gxnvujzmn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gowcsmxks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/ggijnchpp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fktsv.cn/Article/details/guduecsmb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gkggurndi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gkieypikr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gndwdxxna.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.yfazqb.com/Article/details/gatblzzpu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gzkyuzfhn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghitztqls.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gctmnhwtx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gquiqvegi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gxgzvuoqj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gjdugeumz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/glgfauckm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gsdjhbeps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gaassycux.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gooywpvyl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gbuzxywok.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/gtwjgehvg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gpnrhdjeg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/ggkkaqiet.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gnqrrxbqs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gixutdfme.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gpufqupau.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gdphnijvx.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/ggmvghwoj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgevqwpu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gnsavcemb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gtorgkwqe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/gefpkduro.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gadppewnp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/geewqmylc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/glnikmoji.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gaemzbqpj.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gmigrnbxp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/gwflpkfcm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gzwaskdiz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.epnwcf.com/Article/details/gjpojzzjo.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gbkkpcgsh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gprlljmgq.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/gilrbyjsu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/ghlzycvps.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gqvsigvnt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gpttmqpiz.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gqvjqnbxi.sHtML

[P07] 防抖与节流
来源：http://www.m.share.vehdjk.com/Article/details/gkuxrhphm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gfthyzqey.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gdzmtymsz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gdogzpfoz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/glpxdfbwg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/grvuagehs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gszzmmknu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gqbgjonht.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gzejitgai.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/ghmnhyblj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/gzuklwwps.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gtdxrccni.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gjkqduqth.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gukpxqbwh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gqmhiwvrz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gwezjfgfn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gydkrsiut.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/ghwwqvfru.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grifgqzgn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gwlxjezmy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grspzqyok.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gisszzfvr.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gtaiuuwyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gyhzldtlp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gabhjhssg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gayuvjiii.sHtML


<!-- 参考信息 -->