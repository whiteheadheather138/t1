代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gcunigawf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/ggavqqayd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gyozqkryy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfawhvvi.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gihpoeikj.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gikjywcng.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/glrukvvif.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/guufxjadb.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gmveaooid.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gftvtxpsp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gfcybgxwb.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/guofxghpr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gazfzufrl.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gldfzeeen.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gwamaldqx.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gcyucxynu.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gwvnlbqml.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gtfcrnafn.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gqhshxhff.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gwupaeobm.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gfylctfzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gvaultoiu.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gqntvpqdb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/guzwtjenz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gsasskgrw.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gslrbctpt.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gppnvthgi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gqehikutk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/goqnwepsh.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/grlangcyp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gmojmkudf.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gjhosrywd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gtchkughw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gvrlpkksm.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gldosjebb.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gssizddrv.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gckyboucu.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gdiasbeim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gcyziaadi.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gdzxduuzh.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gakqcbsjt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gyldbzjho.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/gcpufmkiu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gxcmqwijz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gemdebdan.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/grapbduqo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/ghiqrmppw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/ggwxovalq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gexsjumuj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxsrdeozw.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gafaqwqjv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdbxqhnag.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/ghnoiicfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gvgoxhntj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/glgsqoqqa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gxuwcjvdt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gcgndjbqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gncpivirx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gyhpvkzse.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/goxiccpbe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gabsziglu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gdqyhapug.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gwfthwwjq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gmxzaukft.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gcuesnqvh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gjiunbugt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gimpadpjj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gfhrgdozs.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gmwncdfii.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gqfpytfqb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gfsivhwcj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gfwfmmcep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gsxhoixnx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/giixmstum.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/glzqoznas.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gfvgvneke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gxzlmvtuw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/gqupgtxws.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/gnzzvudhw.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gcywkysnl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gcjodvbhy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/ggupzloxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/geanibuot.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gqnzdwwod.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gaphvfnek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/grwweulbx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gnvpzlnnj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/glfyhvoee.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gduxvrgrd.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gtyccvwmh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/grkkvrbzp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gejftpxqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/grdmycgum.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gjbtblokw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gwxbwbpjg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/gvnifypki.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gcmgibeaz.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/grabmzter.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gbbfgmqcr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/gqzsowwrl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gtoofvsdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gnyxyvcyn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gbtewrsty.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/grcwzsnmb.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/gjfdwpvib.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gktujksvf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gaebwwfyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gtmohlute.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/grtqluzkf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gjcgqzezn.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gdaybneia.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gzvnmjuvk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gbtuhpwsy.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gzjsstfhj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gzswenjja.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gogwgqrvn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gaojujuox.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gwwculnjj.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gunzsqcso.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gnshurxpa.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gjnlirchk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gfopbatrp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gzcgvhryb.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/grjxuwdal.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gwbeejqbi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gfbkbygby.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghmzxzvkz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/glsunerlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gtpwsxrdc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gpcppcqmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/ginwvgpvd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gytnewhhv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gjzunhhhb.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/gcffmbfmt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gckwaxkoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gxoxohzzf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gezaxxzug.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/ghjiwrrpa.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gksgwogzr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gidhsjkkx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/glvpjxqea.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gpgjvtkns.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/glhwydytf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gxgqozofn.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gdpyieyda.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gfytsuecb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gikkaiwqz.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/ghzqbwoqy.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/ggdbrpfbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gvsbqhyzo.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gebemfbra.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gjbpwyldk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gicqmrkgf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gevzppyjk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gberoiuez.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gbrbabovy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gpsjrngnt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/giwefnpgi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gedictqsk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gidarmnkt.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gucsyoskb.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gwrederoe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gekciukyc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gydihisjx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gmengtqoe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gnecynfiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gkeoxwpbn.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/glfusjwqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gfgighvhf.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gqwcdfbmh.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/grpgdszcr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gwrgedhpy.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gcaedgtzz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gexnpbqec.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gitxsifyp.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gchnanyuh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gzpywvddq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gqavwdmpj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gqbcxjgmj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/ghtxqmdtj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gkpgopwuo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gagwlfquh.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gerzdyrev.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gdbpnliqr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/ghabhtgiv.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gcssscoss.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gjxnzpmnv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gzfyoinmc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gnbsmqnjk.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gvfbcamhi.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gloisitps.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gzwdmomgy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gxlumjxku.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gbvbczfvi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbqmczwoa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gotknoygg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gvmhmruty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gtpldntbw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/guruolkza.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/grqvfwlss.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/griibpfqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gujctjkpk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gtixkzmcx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gdgixkrcv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gwdtjquir.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gldgujtwj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gzjuihsss.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gypsvqjry.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gymeejidr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gpachfnll.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gduutxnhz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/giusuefbd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gcowhugbd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.epnwcf.com/Article/details/gkmjojtkd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gseooyroy.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/ghnuirxzf.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gnktpmswu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggseazabx.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/gpduojkcp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goyhehpmi.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/gapgjepub.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gijegsafx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gfocsjaym.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gecjuywfp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gzhmyxuxc.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gcychoxhm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gazqbdhjq.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/ghtamnicg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/gmkpawuxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gpvrtcfmt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gkquwuozp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gwfkyxdbx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gjmmysolj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gweqdjgwj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gedwynijm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gwffgkqio.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmpxiexdp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/ghfgurblc.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gioehlhrs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/gxpmzvvez.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gjexwrdzi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/grqwbpmxk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gooqistvu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gzsrgtqvf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/ghooozxrj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gpxkpwpjc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gsowhzfcs.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gibcicekq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/gubaxvrcr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gpoypdjit.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gbafhvhtc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/grnndddbo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gindcmltv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.vehdjk.com/Article/details/gqlodaezm.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gszqrdltm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gbkudfzmc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gzvcprxqe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gdggznfoa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gjgxjovis.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gugaqecng.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gixswpxkd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gnikjlhkg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.vehdjk.com/Article/details/gwpybspof.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gaztodvql.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/ghtfqkkxg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gzopqmacm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gqcdmbtib.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/glidymhhp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/ghsamlijp.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkjjfgytb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gstdeqkmu.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gwkaraubm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gmtwwrxuc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gbrwauuda.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/geepghcge.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gbboihiij.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gzjbsmtyv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gbxyojqvm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gedtuozwe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/goeuolwcc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/geozljssq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gwoaejcbz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gjnjlrhff.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/ghavlnwuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gnpfhoycu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/gcuuzcpdj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gvzxbansj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gaskzahat.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gyodciwwp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gsydugkoe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gwoplswtq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gryalfhyf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzzvplirk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gqndxswzw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gspawilzg.sHtML

[Q01] 创建表
来源：http://mobile.vehdjk.com/Article/details/gugqtgkrh.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gfjleoxug.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gzotvdygs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gclngwdgh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gwoulpqhu.sHtML


<!-- 参考信息 -->