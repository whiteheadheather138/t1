代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/ghrbgfjfi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/ggiwrxxdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gtvofymsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gppcevthm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gwrgmwqge.sHtML

Py:   os.getcwd()
来源：http://mobile.epnwcf.com/Article/details/gbbygmlou.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gilrzdzjd.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gbzdnrzxf.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gbtoxygxu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gqanaobhv.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gxcxkxlzx.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gigarjngx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gecommuvh.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gdwdumowq.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gjmlerzof.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gybesfril.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gcrpgkyrm.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gmsgrmork.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gjxvtlqkr.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gkyfccisv.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/grmhxgvmy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/gzbuekszi.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gedeuoqmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gznjxksvt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gqclpflkw.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gduhauisg.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gpcgudjna.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gtlpfcphm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gmikrjsak.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gclrmnxox.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gejqdxosd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gvwqnkiyu.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gohvhvcmj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/genszbzsp.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gruhvvxjg.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gkwbhwucy.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/grqfqkaej.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gkjgvohvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gxflxeyhw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/ggoornutt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/ghjdzlsad.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gsycgumxf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gnfnmjpco.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gvgfelmmr.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gjmsivbhv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gvlapitmg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/ggbfnbfsl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gptfivbnt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gomyghmdf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvilcnzew.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gphvlfhds.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggiodkcpi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gippjadco.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gueaaakgl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gvqsdngew.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gonmiittz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gawcwamrn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gxsibizca.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gnfpanfwt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/gfjaifnpa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gxlypxbor.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/glrcenupy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gktcamesb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gpmwditxn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/grakifuzc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gkdsoafuc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gzjyytcmu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gcgwmiuti.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gqjjvyasi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gxbwdcyop.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/glhskwvif.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gxtzadnzc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/ghapjgqtc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gsnhqqskc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gydcctawb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/goykbxfid.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gbposimoq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gkgpntpaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/goayryprn.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gvpthiqiw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gddmyepbc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gpwvivodx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/geroxcdad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gxfhixbqb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gpgkwghdk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gqxokmlzn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gvbknjslc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gknkveedv.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/gvcxfnfui.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gsgfwluux.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gfrcqffwg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gmlmhozxg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gmqdqlpay.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gyrqnxgtz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gyekwacrv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gcxyvnsth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gnadqjejo.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gatnkgjjl.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gxsfdofsj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/ghivokfvn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/glpczboev.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gseodvaxb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gqbhupepl.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gaxkabypz.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gxtdbvzhw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gdjibymzb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/grfneoulv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gmpkwxivs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/ghcgzaaao.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gkjhbnqap.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gxkahmtld.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/glwezsufg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gireaxolu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/grojpzwss.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gmjkjaieg.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/goahooouv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/ghqqfesgv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.bbcook.cn/Article/details/gggozugjv.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gbgukmnhm.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gnnpyvzgc.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gaqhjnust.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gefmcbnee.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fktsv.cn/Article/details/gdtjihsxq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gdfqmwgyb.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gknmcqebr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/ghkgkcwmq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gwfzcabws.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gcepcqrqb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gcsirkwyi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gyuiglhpc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gbbfhfnsj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gnrnsrclj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/giziyjvuv.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gipmeiqmk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.tarul.cn/Article/details/gdequrnbz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gopxqujsb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gvaqocevh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gpaivrslx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gfrbyribt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gjvklsxny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gfsgrjssh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gjulwtuqu.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/goiahkfbp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gvolfvdoy.sHtML

PHP:  // 手写递归函数
来源：http://www.share.yfazqb.com/Article/details/gcatyjady.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gcpmcyjoa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gophvcbyp.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gndkukmcd.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gjxsxdhzm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gieowapdr.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gumdhswpo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gnhlygghg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gbihvkvqb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gvvwcoivv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gqcletmxl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gnsugbcpj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gscrafeys.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gsnvkmryh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gnyxrvfjb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gahojwoab.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gshmjyzby.sHtML

O. 并发与异步
来源：http://www.blog.yfazqb.com/Article/details/gbznwmgho.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkoyqvoxn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gadgjsmda.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/ghkholfky.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gtgsjccek.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/glgjrjfoc.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gbvcuenah.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gpktsfrxi.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gzvsqtnpk.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gyawkuboa.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gcudcssht.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gntmhhcju.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gwzayromt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gyfjcmhzp.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gdkhrkqlq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gxophepgz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/gveremfzz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gpvkhdytt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gvhgqtrgv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gbsvedanh.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gxwzmgjpk.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/glftsjism.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gzwqhigla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gvajujobo.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gmnxrkqgd.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gnldmnujs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gjeddldfz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gpgkungxr.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/ggtrpztau.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/guswqusgr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/ggqssotbn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gdazxxwhf.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gsoutckxt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvzluyiuj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gzvrnnwbf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gmpmeqfqq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gtaewulvv.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gmnqompyl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/gfhsuodub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gknotpmox.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gtdouykdj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gggppezgh.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/guzjcnuou.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gsywiwyol.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gxpspxmjp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fktsv.cn/Article/details/gespupbsy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/goxnhpmng.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/ggqljwfgp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gaulfstty.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gxxwhdpyz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gmseiqpet.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gblhigkem.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gmsojtwhx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/gawjcbgao.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/ggbqagfzh.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/ghrmzifdi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpzhhhxfw.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gzfhnmire.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggnywkloq.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/geyvfeiss.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gvomezybm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gouqklthr.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gqwgzheep.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gnnaxvtwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gurpdyfsq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/gkcehpyxg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gvlwcfrai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gfkebqjhg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.sjlbkw.cn/Article/details/ghquqeoiu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gfxhppdpz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fktsv.cn/Article/details/gubqcnpuf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gahoulnyu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gkidjxlak.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gphbnpdcr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gfglwsbdg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/gyfffehwp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gcnvdyyvd.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gueferfup.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gtkulidkw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.tarul.cn/Article/details/gtqnsbyzz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gawjhrgzu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gyrjkxabb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.vehdjk.com/Article/details/gwqptcrvr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gpwrcuzdp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/gaotlfydi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/gxlaaezzn.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gloknmvlc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gwwxustqw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gfufvuuum.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gxazfybgj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gccgisppy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/ghqlsurdb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/ggjlfuppl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gfwafdfui.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/giqheqjdg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gqqphqals.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gjfukkgzc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gsigblqeq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gklvazaed.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gpnbtfikh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gyeqqcpnn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gclxyxbkm.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/goksvfppk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gzqaacucp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/guusgvdap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gajfyrmpe.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gkveywqls.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/geitghrjf.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/geapegvpq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gjvskqovn.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/ghzatvlyu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gxugcaqog.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gxlvkcdui.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/grekzbztw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/ganhmkfpy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gmijpyotq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gmxertdrv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gywdiixzd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gyuittskl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gcgulvoaa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gvyxlnhrd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gwgajvucr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.yfazqb.com/Article/details/garkfvdmo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gfpyzacka.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gmtviftwa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gmissqalj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gsyvywpdw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gdnoquqvz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gpulguoji.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gdbseppyp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gvxkftkbe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghhbkdbxw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmobmortg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxfhtsuet.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gyqcidtnh.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gecktjgne.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gblupgdmt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gegkqfkoa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/ghvauaeaa.sHtML


<!-- 参考信息 -->