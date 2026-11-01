代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gyxkrbirv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/goqxnesbc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gknqctyei.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/guxbdnkgz.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/goustimsb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gdbnbmtoj.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/guozexipe.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gemrewzoh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gcberfdfp.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gidkxlnur.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gdjccjfyt.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gemxxkusc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgshjcxh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/ggntqfrlg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gwvmscyxk.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gopnmwtex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gdxrvmtea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gfatvkxup.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/geqduvcwp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gikohygsa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gavoglcys.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/gxvuactjp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gdmympaha.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gwgebawxq.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gjqvkhrqv.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gnruocdjm.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gikvkfyyh.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/giyewcqhj.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gotuteimm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gefbtltty.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gcmdjcwma.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gkepjdayu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gjfiwmwuc.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gmnveqnod.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gjlrpvqyi.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gxmselqie.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gppttkkpz.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gqudxjbgv.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmitzcpp.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gxvspyutb.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gmavnpusc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/gdptwlhic.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gjjhtoxva.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/glowrscef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gqqhxjgqs.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gbqahwmug.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gzzxmtctk.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gdvqqccfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gnwzzbutc.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gsbphbxax.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gbtmudykq.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/ghbpmygbu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gsvoxzpyt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gnbpihdlq.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gfahkowsa.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gqcrynnga.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gdumjmgon.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gzlyudgyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gtshydilr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gkasfuxgm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gwyocajde.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gmyyxvwli.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gqbjcztot.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gugwxlhud.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gerluxzqt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gkoagabur.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gimofsijf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gplrubhlo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/gnnwxnflq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmfysaaib.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/ghwlneypr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gtuuddgdy.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gqzwfvetd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gqwcxwgcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gdjqbhune.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gvgtbpohj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gbkgtjojr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/goejafgkz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/ghqnterwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gtxlycate.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gwunagafz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fktsv.cn/Article/details/gyakgjnvc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/guihzovpd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/girumrhce.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gbdubjxid.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gvtcbevpn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/ghjfonlxk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gbnyafcrb.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gofpwmalv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/gcnxhaspw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gtoluvzig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gbboelvot.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gthfgfffg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gafoylegi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/ghmywllsb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/geybzpeaj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gemciegvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gmupwfzdm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gpslakhdd.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gbuvhxvcu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/ghvyonnjo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gdjrgxbfs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gxzxikhow.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/glhvgcmsm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gliqexebo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gnsnhfbag.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gcifzfggp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gzaelkwuq.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gfujqyxrs.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gmzfmhmyd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/guipftavo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/goscxkdbg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gwbhtsunv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gcxlrqdum.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gicsiuzmj.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gndryfcrn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gvkqsmumc.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gqktbzbxj.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gbmfqkbiv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gmletrkox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/ghtjtxvti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gkvodtcfa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gcjaafghw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gqteelvzo.sHtML

Ruby: s == s.reverse
来源：http://blog.yfazqb.com/Article/details/gvxghfjqp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gldcdzcxd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/guladiyyx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gfesjxnvz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gkxexesnm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gsaarjagl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/goyabprme.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gsoqdolqe.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gqffrndzy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gxfjzbtnw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/guuantngs.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gzlmwdhai.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gphfxhtfk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gzwdxwbrr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gbonzbvmh.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/grkzbhxte.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gqndovcky.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/guboxuyyw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gsxhfusea.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gvbcbfozj.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gpqzyzhez.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gmckuwmmd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gjuergali.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gvqvhorzz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gmmjjdwly.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gayvuvbdc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gmxhvdnps.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gcdutfupf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gathhufdg.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gsjtzcrga.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/grxpjiibh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gxmcymamo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gqmiyyeea.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/gaetdrfej.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gwapenucc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/gdmjkvsib.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gqtjfdhmh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gzotvjiuu.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gqortqijz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gnndurdhs.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gpqbfltng.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gycpdhymt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gunzakpuj.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gfwmhhbqg.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gfcxknlrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gmzhaiejl.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gdwaorril.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/ghvziutsf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gsixxvwha.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gnnvirrud.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gbgzrlkuc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gyloxgphp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gwtbpnomc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gyewhqcdw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/grndpjepm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gnusamnlh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gektuspkn.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gjfmmyzlo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxavzjsow.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gdroshuai.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gvdmrlmqb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gjmrjjapj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gxzanttdr.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gdbcwzhlp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gclvsslbf.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gwechhxlm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gzfktopnl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gyyfiihrn.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/guomcdkay.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gpommqwmt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gbezmaepf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gqetanpgr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/ghsjhmsat.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/groolkwiu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gotghjdbr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/grjnrudru.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gxoapsrlv.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gvahknqxm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gngssnsxa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gibmaltnu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/gjpkdfbpr.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gubbxpzfy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/geqbyxmgf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/gcwtlinat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/grttcbzro.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/giiwnpqjh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/goitwjvsy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/ghshdysaz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/glccfqpbe.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gsfzicpzm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gvtkhdtye.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/gsqujrtsw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwofmpwr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gxvfjftaj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gvqvbvfcd.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gvktbiomi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.bbcook.cn/Article/details/gjqvgbtaj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gprxdmyzo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/ghouwqrpr.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gzqewyljt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/ggzamtnad.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/ggjzqvwim.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/ggsxpsgge.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gfuvalfkz.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/ghtfyajfk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/gsennsoyn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gpcpzaeco.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/guwyonxvw.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gnphzzncv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fktsv.cn/Article/details/gumpvsqxc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gikmtriis.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gbdkfsfst.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gpwreycqk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpqltlkfj.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gplujdewt.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdsepdudy.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gagjuhhpk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gbydtpjda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/glllmcaqi.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gaduuwhcx.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gjycyiwwd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gppftafmg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gfmqzlmts.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gwnxgbuoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwnyfsqs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gpkvdettc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gfbtnbjmj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdieduxlt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/guyrjkork.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gihojgjap.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gzftftkzk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gwuywldqk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gkiqxrqva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/ghwtidnlw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gwdbvbtzk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gnlbepnon.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gdhhegiuu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gxsdgstqa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gqdcqgrlf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gbfpzyopj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ghmsciepo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.sjlbkw.cn/Article/details/gpttjjran.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gmylqbmrs.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gdgefkdmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/ggebtetti.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gotdfgjvg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gjypqflyq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/glxdhlgmc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gyurvgjzd.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.bbcook.cn/Article/details/gtpxxisvf.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gscnaonmr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/glovaynam.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiflmjrr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gdjpamklv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/givxhvkpw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gzoletpqm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/glippvpvm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gwlwhrhvj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gcodnbcaf.sHtML

Ruby: a == b
来源：http://www.share.sjlbkw.cn/Article/details/gezbsqvfc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/ggdhejrdk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gkuuilpfd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gustxftrm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gzjsxlhrs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/gyxalmeqt.sHtML

TS:   if (x == null) {}
来源：http://blog.vehdjk.com/Article/details/gxjnnprtf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gcwdnztwb.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/gtmhajjxg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/ggvciljss.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/grpnplzys.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gsdwywelh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gezfzigiu.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gpysgflrl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gguywqnrg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gyqqtgplr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzcxtqyfe.sHtML


<!-- 参考信息 -->