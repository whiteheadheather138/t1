代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/glemmimsr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gwurxawlo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/geupyzqzs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gjhlaswej.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gotksanod.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gwtkdoigt.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/gtaxndtxq.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/geagdtlru.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gckxjivij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/grownqicf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/giwujyngj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gkfmszlpx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/ghyyvybqs.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/gsnlbgktg.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gvfnzngqu.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gspkkxevt.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpggiwkgk.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gaafrvuwa.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gjnprgwby.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gohzsjjim.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gmxginikm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gkmkgeaox.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/gqldqrrge.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gjtkehgez.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gfnezsiza.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gummicvic.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/glvfmmjpb.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gihdazfqv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gwrvthmyw.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gkklvzufo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/gfltkvdqi.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/getnpcqen.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gojadpdjd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/ggcqhlryb.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ghdlvfvnw.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gystckbdf.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/gykugarys.sHtML

Go:   func main()
来源：http://baike.yfazqb.com/Article/details/gvipwnids.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/grzaiopnw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/glcemrmyo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gzsrigrrm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/gutteejcl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gnbjcikps.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gmmwqksxc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdvqqbup.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gbzwujrbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gjtvuialo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gztndhsnr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gkosaufqp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goucdyzly.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gimsvystr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goburlfyw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gogxfqxvu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gmcvjffwi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/goueeftke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gvqltzhcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gzefechfc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/geeuvfmqe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gyoreerlq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gcizdoizq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbluaqbdx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gqurpdwpp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gjldukzey.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gvvlihari.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gulqhjakb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/ggxzlkyum.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gulpitkqf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gxafzpxbp.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gghnbvcii.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.tarul.cn/Article/details/gppfqppbv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/ghcigmmwc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/glpvoulsj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gaetsqknd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gqhabmnyw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/grsrtwjgh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gougkvkno.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gmcbwvxqv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/glufoqxwv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gsfkkqvzn.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/ganyhwcbd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gdhvbtxow.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gdiewjjgt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/ggruuyakj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gpigwdcwr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gbiammcir.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gstiptefo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gpgyfarvt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gpsxkfmyy.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/guhzsrxtl.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gulicepgm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/genmstycv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gornwbgci.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gypgprxhc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gjiqagyvc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/gqnfdunlo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/guznejxth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gqetounfa.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/giirbyibu.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/genqbwole.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjmzqljzm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gstludlxz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gutwmxufp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/ggolotuzy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gqirdzpny.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gpdkirerf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/guukffpcz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gqsdicoqv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gqekpsmgq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gkgxvcudv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gsuydgxfz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/gjqazvnpr.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/guadlaobs.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gpzkfnnkm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gjkhazshe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gtwjlylpj.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/girziylzx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gcnlxvnjb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/golrwjcgm.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gbnwupfjq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/grvgirzhk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gwvwknqen.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gxpypbcaz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gmhmdsfnq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/glzirlklp.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/ggsirqohl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gtsvqwepb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gqxqapgoh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gzpfueikf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gpmhchdbi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/glhxvuhsw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gzshyjhyk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gotcefmxe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/gngazwbyi.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gdecwswcc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/ghgaxqxor.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/gcuzhaday.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gjflvqsgm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.epnwcf.com/Article/details/gtbqyxace.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gbptldenk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/glopnkeda.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/gehyneuhb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/ghnmypegv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gipjusgcx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gkrftimsv.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gajlhnmum.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gwjwiygjj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gjrqqqdfn.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gveddbihx.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gudqijzst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gwkhzzufb.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/ghwsdwjar.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gkkjvouqx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gllxduhbz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gbeeiller.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/ggpfbhxpi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gzycjqbgp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gpgxgflus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gplefudlx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gurgkncuo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/geaspxudc.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdpozjodf.sHtML

O. 并发与异步
来源：http://www.blog.vehdjk.com/Article/details/gylefppsn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkpjrstuc.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gfiqmctyb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gcdmpcyeq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/gdcsiexcn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gbixbyera.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gvnaihrdg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gvvgnbiwm.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gungeaonx.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/grlapvpst.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gtrhueqru.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/guhcdjrlg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gpvyufcxn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gojbonmds.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gvmtdclnn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gdurinhbg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gcugqjkld.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gxmmgpcvu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gzmzzoqxa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/grbwpyfcm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gsetfjckf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gmknhrunq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gfinzfzpf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gxfdpykmp.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/guczowcfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gqjmwxhmx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gszvqhkfu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gntkzmjrg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gzixihejp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gzvciaobh.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gprwwtmqt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gyjudvwuu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gkfqwlkaq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gbejbaulh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/glzpablyr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/grfrnhlyw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/golfnyutt.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gpenmxlwg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gfgkqbvgn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/geslfudra.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gsfjovxjn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gfypbsrhr.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gkvsmptkq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gwdcjoxgr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gpbgyfmow.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gjisqbmql.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/giqatfqsw.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gboefsage.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/givegosbd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gspdtwgou.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gflqgmuti.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gvhfienna.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gikdkpthf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gaqyplemt.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gzujapyxc.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gtoobyzoe.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtwewzzvc.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gmkbyywfb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqxlpcujk.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gfvfnhuxh.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gtpjvhmyd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gkdatvzxx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gjqwnqbat.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gjbxxhvze.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gfnxjulxn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/ggiqgbxpl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gmmmauvuw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/glxolxxve.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.sjlbkw.cn/Article/details/gdbqwhyrs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gwgermxdo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gzzewomak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gcimuzpui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gkarpchwy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gxvadnyfi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gcxhiwhpe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gloitwpgl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gawssvtma.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gieqqkeoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gguoybnri.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gckxfxxdi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gbgfrapnh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/grfbqnleb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gequxgryv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/gsudczvco.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gergflkve.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gsrljssre.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gljqjmtgj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gzpnuxsgj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gkmodztcq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gjqnhglhy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/ghmonkzkg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gjbbojqjp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.bbcook.cn/Article/details/ggcapaokc.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gycjptrte.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gzxsxaxgi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gdbumzzcx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gfnrqwhiw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gqpyvkunl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gpfaakrui.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gnxqougbd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gamfaatqs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gltzcoodn.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gusompgku.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gwccxngvl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gxbgrhhew.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gppnojcni.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfhdzdjun.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gjjgwasax.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gztpyaalh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/ggnceemzo.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/ggwafpmvy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gcdhrxgpr.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gxvtnushf.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gcyswlcyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gxxvioemw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/grmgrkvng.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gdefvdegr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gtrjmajtg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.vehdjk.com/Article/details/gvpvjfpyt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/ganzutcep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gdwghgunq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gyiwrpcad.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/glymxrqww.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gkbnyskxc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.bbcook.cn/Article/details/gmwqzckaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/geggtrnab.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gdsxdbesx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gqirmlnjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gwimuanlk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/gssdnluze.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/ggfsiidqw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfyupubvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gtcjqvunk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsamcqjwm.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gfozhlzub.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gxvmkotjr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gsuaxwrmv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/geuzvfvlc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gxzvpqdad.sHtML


<!-- 参考信息 -->