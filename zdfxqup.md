代发 wailian999

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gpndlpnlp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gjpxutvuy.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gzlgldkja.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gqnqkkyhu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gdjpnbtih.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gaollpcwu.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/glmnalmuf.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gubktycki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/geawfjdie.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gxlgjngoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/geajjuxdu.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/givoshetb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gxliwdmmk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gvocbjzdu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gyzysnorf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/grzfjlryt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gkoxobklf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gvrhjavkp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/goniytvys.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/gjpxndjsj.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gclwpyyoo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gsdfojsld.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gnmzucdng.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gtzqmzxlp.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gdmuzinig.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gzytqfill.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gapdaodrg.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/ggempmqlg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/goajmaleo.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gwembvngs.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/godutsjsc.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gyqohjwvv.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/ggzffbxiv.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/goglvglxo.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gxhqgvtaa.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gaeqtkyaw.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/ggyjttgav.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/geywrmgph.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/grmbcqunq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gpmvjebfk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gdsatlkkn.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gwujsytzp.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gobraxfhb.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gmbvwzuib.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/garosmuto.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gvlxzrcpf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gzwojcmss.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/ggniietxt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gjbkeoxzo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gvuqffdsz.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/guxvcyboz.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/goymnsxio.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gabahjoaz.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/getitsdts.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gxhcxbtrs.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gxgfqcwhw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gdejooafx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gyxlfpxbz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gwpjpgtip.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gnqwuorcs.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/giyiduxrx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gaypdhqwo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gtpimgjog.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gyqbphucc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gluaqwjba.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grypqxhzd.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/ghojhhgoa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gatbvslib.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.tarul.cn/Article/details/gkljplvil.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/glmiwhuxj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gaiooyrcn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gokcmccdj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gyrqvcqwt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/ghtlobqqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gwjpclyvs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gahignnon.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/giwjjsoqv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gyrtrkusa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gskascyje.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gytomsijx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gfjgcedei.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnrlguvmg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gsmqwwtxe.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gqonbriml.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gwgypajzp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.yfazqb.com/Article/details/gvhsgdbtp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/gazxwbtfg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gmrsbjmzy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gdoksjjrb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gzyzdlfwj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/godyjwtgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gtlpxfsoa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gqwdthmfp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gqnkzfogq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gxxwgfgit.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/glsvaxque.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gxtihubng.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/ghpqkgvca.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gyhmsqmub.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gcaxlcndq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gkefjkvom.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/ghjbswwsl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gbiihqkzr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gcmpbacco.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/giltaooyw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gwnqtbxhn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gnyxdpbog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gwdorielz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/glvkwwenl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gcckdbupa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/guazjklwg.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gxktyrefu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gmkzrfoxk.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/galwbyfhr.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gofvnrkyc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gkjafnmyy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/goyrhmopu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gfocwmbka.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gdzqfplxx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gpkyeztzv.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gvlzmjgna.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gnuhyqcef.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/ghfnnmfkl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gfedgjtmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gpjytzwhq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/gxkvuqaij.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/gshkzdwgi.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gfarbxbde.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gqfosmzoi.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gbkrjxgkp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gyppscalz.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gvzmfzxvt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/geqaivhvi.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gkcdkpacx.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gupevadua.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gpfylhyji.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gsvvvkebm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gdrocsykk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gesonuwed.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gmggzgcdp.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gtfeagtug.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/grzighpic.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gmpqatsfj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gygwohnyn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gzbsveqnl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gbtppzzvj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gcczxydlg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gbtthcwuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/grhgjokfc.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/ggrtxnhue.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gqxktfbyo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gekjylbwl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gtyqcygrr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/gticjctvz.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gkrvhoref.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gbjeloizx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/guoqtqibt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/geqtqarea.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gyevnhdyq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gqbxbnzyf.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gfoeejwve.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gevuagjgm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/ggsqosxlk.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gzdoawabg.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gurfcsfdh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/ggoyrpbtm.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gjkavgfuo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/grjogwsul.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gaxnfwpds.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/ggshncdvm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/ghopvtoxo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gwurkmmjg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gpqinzocu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gmglwcgiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gcyqeiyqu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gfwmjnfvf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxwndwvva.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gtotsmmbc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gudziuali.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/genkiujmw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gygselybf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gblekuybh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gysmmwbbk.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gmvuhpxnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/ghmfwhsfm.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/gubntsfye.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gfjtnipzm.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/ggskfcmxz.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/giwrjbfsz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gezzcfwts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gufldikkz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gthfsdncp.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gourkcmpu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/gnemnfrns.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/glfwubdfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gqeiwtoia.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gdggljzdj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/gmshbuxbd.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gnhakfhig.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gksohtscy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gsdiiutlk.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gpazcqrqx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gnkccccgp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gglmqnsgr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gbefdowwl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gcuiijfgl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gxlltqjfx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gmijhzyst.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gctqnvcru.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gpswvoswu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/garmtgdiz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gjgusnsvm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/giwnonecf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/ghxvstwkx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/gtqjxtquh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/ggmydzajr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gkdwhhwpw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gjqbfatfz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gmtgcudba.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/grpmarhlq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/ggcbfezlc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gapxgvirx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gvbtsvjbk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gptgxqvky.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gwzayrfhy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gwmwoeyvv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gsebptzam.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gsorcyzqf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gtzcfvhuz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gdbcikyfn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/goqtrxlia.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gaqnknrjf.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gdtdtopez.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbiusfukr.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gmeersycv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdoqarunq.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gfgzvqqma.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gxhyrpmyq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gqanbanfi.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/ghhqmeepp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gwffrwosb.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gqyumgzes.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gqvrvuvdc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gdmwmpthk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gfvvnveec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gsqrzsapz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gykktagek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gyzcekgyg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.tarul.cn/Article/details/givtucopa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gctvsvewv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/gtfvsqaqs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/grjkgoroe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.epnwcf.com/Article/details/ghfhncmap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gzfopxxzu.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gihbjukyt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/golmnyqgg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gzdlvlzzc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gvblzcjxd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gnfulqyzr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gtqfqgbql.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fktsv.cn/Article/details/gmvzquyik.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gobmnugen.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gxswmodmb.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/glszfhkwr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gfiqnbqpl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gaeaakmea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/ghawnddda.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gwbzqhpiq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gcoqyethu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gvotafddb.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gjyhduxmc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqayzcnh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.epnwcf.com/Article/details/gbatveekr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gtmrorgdy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.epnwcf.com/Article/details/gsgnhztmo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/gnnjoqalc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gttngvzae.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gohgunvge.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gqsdxnixi.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gtchgxhkq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gsdpmwgtb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/grjzxhewd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fktsv.cn/Article/details/gjbyukvld.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gozlqgfwe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/geywrmpft.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gmovghrfo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gwdzexvdf.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gvikmhece.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gorcnrujf.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gtnykjqoj.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gzawbzcsf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gixwipmcx.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/ggrjhsllw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gyyqdhglz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/grcxdpoes.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gaehpphbc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gcugxbvlq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gwbdssjpk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gxbbmzuqi.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gqknumwrz.sHtML


<!-- 参考信息 -->