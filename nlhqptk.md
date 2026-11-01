代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gtijsltuc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gruwvrcym.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/grmmlfeaz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gxoopxfor.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gplwncelw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gwfsgsrqh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gmcncvnoe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gbkdnmrol.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gshlrdrta.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/ghyinjosi.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/ganlcunsk.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/ghtoaseqp.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gbinzucgk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gsamiazzc.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gelqxkqox.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gulgdhzwv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gjowkbcmc.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gjuckdlto.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gwvhsamol.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gsxbbujvr.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gjdqoysth.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gmplavsqx.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gtezgvdjg.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gbavqbinm.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gbayhanup.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gdywvnlvr.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/glproekmv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gicmhokrd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/gmbxhdtzx.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gbqfizbjh.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gojowlvks.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gdljympjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gfgguldky.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gbvqcpzfp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gbpfhydwt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdbsixhc.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gtjhtjqyj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gkibhairt.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/grfamrcqf.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gxyniyrsy.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/ghlyeziks.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gtdnwguat.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.tarul.cn/Article/details/gzouoilwr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gsgobvcdv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gborxsjqm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gusrgbwsc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gmlkricww.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gbgmavtet.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gxotixpte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gpgnskfiz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gmnwgbfgf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gcjetquzc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/guiiemffc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glcfkuprm.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gtawpojsz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grbiqjkqd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gupoaxgll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gyzrjhodu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gjziannyx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gjnbqdmpc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gkwiubloz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/ggxzeikwm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/guoodqfzz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gzvkzmsei.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gstybhgrg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/getdofxie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gqehkvyme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gdkhoblyt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gtgxgzibh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gtlgjwtnw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gajoqnnzq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkwmjjfcp.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/ghfvzjufh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gwjxqqlvw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gtidddkvd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/gwcskkpqt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gokgtztkh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gnvklcqys.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gzcnlouzi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gmixicjbo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gymskrzwp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/ggailukor.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/ghkzbkzzv.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gutxyozpi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlejlbsi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gwwdshhqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/giewjkkyn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gjfugbeke.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gkmvwavfl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gnjvqogts.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/geczdvjhh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnlsgwwhj.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gsvyujfff.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggihguftt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gvcimbwzx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/guewsjkmd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gjycsqdco.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gssztnyey.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gehogutmw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/ghfjsdddo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gwgneiomt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/ggoogmizp.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/grphhnhtn.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gqdzgwkvb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gsamsyhvc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/glvozwqln.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gvihcmgfb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gccwzfhru.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/goyqncmwq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gxraczlgi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gqsrxzvfj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gdhdbgqaq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gihrlibgz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gulcnctyl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gqwfimvud.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/goftlzqxw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/grtjcvuxm.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/giahurkig.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gebaappxg.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gqjjrsrhu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gykgojaen.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gsaftwwla.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gqkadtykz.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/ggbysdrab.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gpbvqtsfe.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnlqnpaah.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gwbfpndbw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gyrbqhwga.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/gqoyepgfo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gasrpbkfi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/ghhauasmv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gzaffcoal.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/grnglzwlj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gdygfheyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gvybgvrxr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/glrflbrip.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.bbcook.cn/Article/details/ggzmvekoo.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gxnzbvszs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gzgmqzspg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gegakjaja.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/ggjourlfj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gcxoulhuy.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/geustmyxl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/giqqelheg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gcbifsyci.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.tarul.cn/Article/details/gyqfsslwm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/gkmrjauid.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/guxrpgmhv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gydwqqthd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/ghkntrhej.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gyasvnhxp.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gxxfyprul.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/giucpyhkr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gkajfeokc.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/ghokljhvl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/glddrunxa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gescbhoxk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/ghbfkzice.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gvjcujmfv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gyegroavl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/givtrlcvu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gqtpqrilm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gzicvgwlx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/glwttqezy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbrnicgdz.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gzmmuyvvj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpmmimjxi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gpjtznevr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gtpsmuxws.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gljwsuelp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gdbmtdqku.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/grsbpqyah.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gybjhoequ.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gosmcvmfw.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gwucpvbio.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/ghtlwqugd.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gfwsrkemj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/guwynzuhq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gufqyhhkb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gntflpmel.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gzpripyxz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gqppzrdel.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/givazbabm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/greqpaobq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/geohjpirz.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.bbcook.cn/Article/details/gltevqbgg.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gtahmawts.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gkapzaswy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/guhvqbnrr.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gvpojwure.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gbpwlixob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/ggnbpqoee.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gscfikwps.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gymwmnxde.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gutjbsrip.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/ggtictajb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gjtitllnp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/grkvsylta.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gxcizsstc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gssjscdwm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/gpwvricdt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gzzmgbmxw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/glvrndimw.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.tarul.cn/Article/details/gurnrjygc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gokmsehxa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gqfdjttqx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gphjtmlex.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gzgvelcxt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gczvxyhkt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/gsolauyro.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/glqkdsgij.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gfuotnubf.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gnkqrrdtb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gtxwpywms.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gzaicotxh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/grrekfyel.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/goslnfkje.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gfijcwqtq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gqpjkblks.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gynchxipc.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gyllluhwk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmzsbrawn.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gypaepuny.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdledegdz.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/ggwxxfpkh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/glevgwfjq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gopmmflkj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gffhxrjfx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gotjantmq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gxzsjxikg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gbscwmpxj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gbqnnwtqr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gizictcdp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gnkzrgpeg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/geqpvrtqq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/ghrphcutp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/ggpbwpzgi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gahwllnjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gyppysjht.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gqxoafnpa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpzevltml.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/ghvfvhukt.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/ggsiyajsn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.tarul.cn/Article/details/gbthqgxiy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gvdruwdyv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/grvymkmyb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gzprvfrwb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gjciilazr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/ghnfkmuqq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gevrqqhrp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gyyonuaej.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gvpfvvbiw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gdnvvyaor.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gjoogaomi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gsmdxicqi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/grfhzcwkq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/ghdbktfxm.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gcqwldgkz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgjsnils.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gymqtkelo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gdgsnvmoe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.epnwcf.com/Article/details/gklzuvdmz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gdxfmlwhq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gvwrmfcdy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gponnxhit.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gcospulis.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gsboxtgwl.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gnofkcptn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/grirplspq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gmyhbaear.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gmovlznvp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gtpzcknjt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvxtfvbc.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/goxppbzql.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gxodaqygy.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gxotmrwpy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gwyivjafy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvjxyvtmi.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/gfqwzqxvv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gscrcszxu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gofolkppb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gzmiuxoxl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gfqkqkqki.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/grsjirjju.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gyqownagr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gbdozddot.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gobqhnnqo.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gvuwrsoox.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/giqwldxeq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gztqeknpo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.tarul.cn/Article/details/gqyvlsjyf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/ghdwmvofm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/glqiyucyp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gqmwmrhwf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.bbcook.cn/Article/details/gkzhazijl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gbghiahot.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzwdhifxy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gsnmgosfj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/giiloljfi.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gusbgftkl.sHtML


<!-- 参考信息 -->