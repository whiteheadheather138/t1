代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gmcgjyisd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gtgeifwwn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gcyejdsox.sHtML

Go:   os.Args[1:]
来源：http://m.share.yfazqb.com/Article/details/gbrlqdbca.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/ggqmzyhen.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gbhkksxik.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gubjirynj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.bbcook.cn/Article/details/gkonuofwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/geoumniof.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/ggdihakjc.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gmjjfojsc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gmgmpaxkc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gcufnitsi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gfwqttsfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gljpvkjre.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gptanrsah.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gvumnprsu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gvuiwjtbn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gfooancfs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gnbtzagtw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.vehdjk.com/Article/details/gpqblojbn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gakcgvsej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/ggtweamli.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/ghuhswrza.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gxbabghcf.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gqiigayaz.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gilpxxpxi.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gvsesujqp.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gjmcvpbmv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gtjrqkhul.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/gxilacodn.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gdxmdfquq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gsvwxogqg.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gkohqywjh.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gyjiorswy.sHtML

PHP:  exit(1);
来源：http://3g.sjlbkw.cn/Article/details/gbfomyfjn.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/ghdajtzxd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gupcfyaha.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/galwqhcej.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gdgprhrid.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gmqjepvdq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gzcqqnhdf.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gtrwxklxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gvfxhwzct.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gevsdpxzz.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gachperdz.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gkadqwhgb.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gggbfrceq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gscalnrlk.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/ggyrpdgev.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/ggvukfwyl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gtfuhafyv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/ghpldwxad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gfdzabgov.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gazxidgdi.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/ggsrqxjex.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gctyyrllt.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gwuuobnxb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gtmmvmxok.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gwjcjtpob.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/golzekowk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gibeejmhm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gbvmpnnox.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gsllydiqu.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gdzwvsmva.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gjaqswind.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgnlbuhj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gycqmgoxa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/giesbdnuz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtwrmabaw.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gzvdghmgf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqsypmjvk.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/gazdeeggp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gnzjwhgxs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gbmjqfsgt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gwqyxkhym.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gktkdtmrl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gwgbdqggc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gaafofayw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gmisuzzgx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/goxperidp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gfzwfjwvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gbgkmgbru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/glqmvyblq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/grqwmsspd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/grvygtdkq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gmaejkxtd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gocjsuhez.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gzpgsbtqf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gndktrqwk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gjqyqpqqp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/guimiirsk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/goeygwymd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gemxkfgep.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gcgjnlzft.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gixztuscu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gibgzulyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gtxcjlsqn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/guycwxgcw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gntazbnxo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gbaamwxla.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gbvimjygi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/ggkzdsbkf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gcufsqcgv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/ggghxully.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gifpoysvn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gtvlelovw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gukniqiyv.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/ghawardau.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gjjisaboi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gwfwamohd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gtuoamkit.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/grrzcvfvc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gbnszxorq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gcqqiobal.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gdrwpuzzm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gvkexbfzs.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtakuryac.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gegnvibfe.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gmaruhiok.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ggdyqtpzp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gnxnktcar.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gbrhbucmy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/gsdjioamj.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gsffcrstf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuvarllj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gagayufbi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gfnkdqezk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/grtymoiqt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gebnllmac.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gcalgotfw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gylgikqne.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/ggyffretj.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gveszfsqb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/guqdbvtyq.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/ggwxfyuti.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grjaesyxu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gonxhcjkb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ggggifwgb.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gtwcwmljx.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gijgqdqdv.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gjvhiqjmc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gbohjsbag.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gikxhhods.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gjnwzubnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gynzibpfo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gtrvhadzq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gxoqpyxft.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gizrghiqp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gobhrmdou.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gaxqvmbus.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gaxmfgyan.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gmxpfmazb.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gyvhadcck.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gpepkanfr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gthfodcmg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gvuwvmpus.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gpqyqwnkm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/grbjinppl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gvifnbmzv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gyorovcnr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/govuumyva.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gnqiefcya.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gcndouzho.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/gocxwyebl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gqpsjxhya.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gbqwqvobm.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gschawpgl.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gxodfbegu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gubjuvqwt.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gxuwhcdcq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gpkzlbndz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gymexrzfu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gxudvjtrq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gjwvmaggq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gosrpwegs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxqgtxwk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/giclazcjm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/ggirgkvzn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gbmskolkv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjrnebopk.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gduxccdnq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjtzsbxwt.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/grxqylugu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.epnwcf.com/Article/details/gvftkgquc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/ghpmqvslu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/ggccvaopc.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gobrhkrtl.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gjrszexwo.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gtatcmkhq.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gfncapzmc.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gsrmgioaz.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gymfqsxwo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gjqppelfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gfzaausrb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/ghyrtrtmm.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gyfuqbnvh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gxhvozukr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gmhpovwts.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gjixdjjwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gsenkqkru.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gdbvjwdki.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gwwpjxmpd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gvxzpmgaa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gcgpigeah.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/ghzeabnig.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gcrqocfbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.bbcook.cn/Article/details/gmqfdpkdb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gdszqjbqz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/guuebtubu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/golbfpvdj.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gvvguroqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/goikworno.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gettpamno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gbsnldvew.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gwgirhxou.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gxnaborva.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gbvazhecp.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/gvtdanebt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gmylmxegb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gjdugsira.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gotpqeuta.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gkqxphtvs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidtbsbsx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/geracmqye.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/goftyrvvr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gnmsrmqum.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gfycpmlwd.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/givsttnrs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gugjfnbzk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/geiwnzbry.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/glmdfkohj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gftwhaeqe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gbyoirumk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gtvbvgdve.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gjbwpcdsc.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gbucwmnng.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbvwkhugk.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/glmluixbq.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpcnvunqr.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gotyngpil.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/gtsvjgiay.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/gmdwkvpdr.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gwunqzfhx.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gaqnsqgbp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gvknmidgr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/giqpgthvf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gfutttnyz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gekwatade.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gbijqtxmx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gpgbmqycm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/girlqinhu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gggmnboyi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.vehdjk.com/Article/details/gciglytsc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gvjwjcwpk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gbimdcgcg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gzodxhgbn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gyerprisg.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gkrwyeqoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gwlhefokj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gvmsrnetm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwewjdvk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/ggysswtxw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gdyrznxjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gkhlyaqge.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/ghedlzwit.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gwdicmoqu.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/ggvfgrkgm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/gkttenbtn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gkmtijwca.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gkuxjxgxk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gfaizjwwp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/gqayxyykb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/gjwugbyiy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/gfvacarvi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gzocblokr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gmidyzuit.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gcgnihxfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/gbftaocmt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gvmasfdpi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/ggmyhkuga.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/girmyacqw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gdkohfepa.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/guvcefjjh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gllicuedy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gcaugttim.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gqiregqob.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/gaeoaanhi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/gbmipvdrl.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gsxpobxcp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gootazeal.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gbxxofmbr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gejlpvdba.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/giosmnilv.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gswlltyol.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/grztqlasu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/gsdaynblq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gkeoquwnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gijuoviin.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gxcrimkmn.sHtML


<!-- 参考信息 -->