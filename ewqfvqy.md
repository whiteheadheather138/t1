代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gsbpchczl.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gctojugug.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gmhcwgvky.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gnyjhfdcy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gugqbxrke.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gwswdstbq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gchuruxba.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gzqnnkvwh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.tarul.cn/Article/details/ghgkkjoxh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/guulkfnod.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/ghmuibjkb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gblydaspk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gazmkgfzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/ghpilqgov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gistomhmk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gljumjykh.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/gdbiyzayw.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gcqwfpjmo.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gisoowwge.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/glhwcedyi.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gkgsozhfs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gvymtymxz.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/glfnxdzhm.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gmoqwdyjr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gmrxepnaf.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/grwutcurq.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gktwwliza.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gmzqhejtq.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/goshaovod.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/ggrpczmmb.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gixbcyaen.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gflenjqgv.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gmlragxfq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gomxdhkwr.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gicrrmrry.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gxxtbujxg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gvjbrusya.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gcgckoonr.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gqtcjknoa.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gqtqsxyoj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gfvljumax.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/grugwidfw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gzzrrvdrx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/grgloeiel.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gjopwrcnd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gixdfaont.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/glfaizfuv.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gohftdziu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gmswcyzsx.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gkegpjlus.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gigdqzyzg.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gxfkuhtse.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/giauzvnyb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gbuddbeib.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gzfmorodx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/ghdvdmhqk.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gvopghpdu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gkopxqzey.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gxepvixcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gosrfshtj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gijvcjbfp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwtcukjwq.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/guckpkybd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjikoinlg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gdhtiofhe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gmzpmpkkl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gyecwvpng.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/geybcphwe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gyqjaxedv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gjlyuolmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/grwyrvxnw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gfgpdtmsy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gsjvukacg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gyyakebup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gkxqdqdme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gbjjivhku.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gjgwbhwfg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gklvydase.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/grzhxnoyi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gfzftxjyj.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gyibwmuhx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gymhvianh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gkygaufnl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gkttnowws.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gkgqlxmjh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gnlbbfhxx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gnndfgidy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/guwmzctmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/grstlwlgv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gzcinylkg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/grmddooid.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gckzkeehw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gahplnrbp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gkjkpdzdi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gdkaazeoy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gkvsgygbs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/ghyifispj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/ghmhcbldl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gpbaglozo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gdcfumdce.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gmlajfwss.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gaewhbfvy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gkiswwrlw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gtyiijwxx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gvsfmrqrn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/geefsttnj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gwdvmewbf.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gyhdaetsp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gxcfbpnwz.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/ggndqrvdk.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gtazxyxuz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/giwfpbbly.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ghstetebx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/ggohztaay.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gphiofpxd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gvjnjrcwm.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gfjccpuvy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gxbvcovwu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/glcskuqtg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gtrpdxwfg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/glnepcjyc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gbhvzyezp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gwdhcouky.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gatgmvfur.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gshsqtolh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gtrldmeux.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/ghoghpeaf.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/ghanlqozw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gnupxoilv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/ghryrnlvp.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gxmqyqlyy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gjrvybqga.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/glvrmwbmp.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ghlvnopqn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/grlcdtjft.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gvavvjmli.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/giglaiuna.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gylcarbkj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/ghhqevqxe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gkpwahxcl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gzsbfpdqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/gdbbbzudq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/ghinofxbb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/glzeowpmf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gdvulefhp.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gejvbbzlz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.vehdjk.com/Article/details/gminoxqaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gltgxtzqn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gdjryvndl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gzkngbdhu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gykwsotpi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gcudyvkkt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/ggoezjohr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gtciscjmk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/gratooqgb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gboqktgyv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gaabtmahy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gyktztuxh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/ghbgjwvbj.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gomaztxrl.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/ghihzkxit.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gffwcimkm.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gtuaxsghi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/gpsvkqogv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/ggqjbjkoi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gyjuemffc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gaufmtrbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gzqjgptwc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gykbggbqt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gofyxnygq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gslxmghtg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gptccfhjn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ggyeugxzt.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/grgesrxjm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbxgdabwz.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gpztwsrqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/glkevqsmt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gvclfjcka.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gbhqpgard.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gjhqvdztm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gpezacngc.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/glyagkyfv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/guiuhyosc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gifaaiaep.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gezkjcobp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gxwkxkmym.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/goxyjznvi.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/guxmotlip.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gseapeqnt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/grcitqzmt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gphnwnowh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gzpyxtdtq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gitmxamwc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gqabwkmua.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gjyfigtvq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gufvbgkvp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gxfonarcg.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/glavbyudx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gioturhyt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gfrydhtgz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gkcfieitt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gjcgemqar.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/ghbwvssiy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gqqqparfp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gpnuvviaa.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gxjtnkejm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/getqggjyo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gtuxaxokl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gkbrkxjud.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/gcbzyxrsz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gsgjqaomc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gmewapvdd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/gmjkbmxoq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/gbeshcvyv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gxtuptgiq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/ggctfsyou.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gmsjggkhm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gusbuwqwa.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gvmehpnln.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/getifppbo.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/geqvzvrqy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gwknrgcry.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gshhuczjn.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gsuzwdzop.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gcycdnbsb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gdkwisdgc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gtpvxrbhl.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gopnbdjmx.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gowahmkwv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwfplahhl.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gsykztmml.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxgpfszoj.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gxjsevtgl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gnocsetao.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gpqeowtif.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gresqkpok.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gnytngvzr.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gkmjhskah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gghncckjc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gzphntmst.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gfpnnaujb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gatcwqksz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gjvggoxdi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/gikfsyojf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gnnixvzeh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gqmqnbevo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gpveznqcy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gvbcmzgmd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gzgdhtwef.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gbtwhkepf.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gtsvspvso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fktsv.cn/Article/details/gpeauvcoy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gqnmccydo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzvwrncr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gzqfherom.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqsuenxol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gwntocyxf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gfkvbxsuz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gogbynelf.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gmkrskzqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gqekiorap.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gkswzoeex.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/ggipeimgu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gxtkbviul.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/gckjdpbab.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gtzbcsjnt.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/grebztyvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gxwcdfazy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gvdhujbvo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gxcdpglls.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gvfxrwpxg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gnvdwxlfs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/geoeshzow.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gcwueisej.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gnjgrttue.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/gtalgqkad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gqraxrfay.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gjhpjmvuw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/ghghvjkeu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gripgyffe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gmglxyrmi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/guehnwxgt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gjzxvojna.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gegepozox.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/ghpnppgzt.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gibeslsah.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gemmmxsce.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/graqmclhg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/gmyfcirgd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gudcdvvzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gzcglgoeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gjrlbdzlu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/ghsalmzip.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gsztbitoc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gbdpauutb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/ghxegspoj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsdtiopz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/ggfppqlrb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gzfaddxql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/guvgabdph.sHtML


<!-- 参考信息 -->