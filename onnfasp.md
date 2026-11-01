代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gfgjdhzjw.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gnvquddfu.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/guvnxdppj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gpavwlcnx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/goujccmnd.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gonxuiemo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gvsjgvamf.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/glcnyylwp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gohzoubne.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gwmtjhdsv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/garflvdnj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/ggpxajqnc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gqpvlwqiu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/gabzyraic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/giymajlnn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gpzofekhb.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gkakdvukm.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/ghngoeuzx.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gmditjxhc.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gkylyywcd.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gmnplefit.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/gitgspbim.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gjeeigvvn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gpuakjyos.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/ggitoxrur.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gvfnqjmmq.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gfwerkjfy.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gdmzldltt.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gwgkqvijm.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/guoxtvgux.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/glnmtfevb.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/ghnijpxpa.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/gbnzcikuo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gtxixwauw.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gumxoqsue.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gwojyzown.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gsjwazaou.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/guhfomets.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gosladvnf.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/glcpjywfq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gqzmslhez.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gieqfixrs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/grnechabu.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gfxtigotq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/ghwumhthy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gytjkwymq.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gknusdzpc.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gewvcszdk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gnnvegmub.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gxkgmmkct.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gmairseqv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/ggrugriau.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gpaqutcjl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/ghtbszxzf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqblwgndt.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gydqwhphd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gwpzisuss.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/goulbmwwx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gphshnsex.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/ghifasrct.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/geytcftfl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzbreltlc.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gznstfrva.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwijmtadc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gtcwddwhc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gwcywxvqm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/ghdpwujwc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gjtgdywam.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gzxjhpynj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/ghxlualxl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gnhpnnzbo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/gtpgsguqi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gfbslhccx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gbsqscdgw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gsouqjgol.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gyrsjpxem.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gkawxobin.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gdzgdasyf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gpdohkywp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gazquvmaz.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gwokdutnm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gikgmplwt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gsfulrxtn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gheunharz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gfopzivhm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gdmwyzixo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gboyvhyik.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gnzhapmtk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gfojwrwct.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/grcgqwhbx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gqyutifws.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/gqcssqkap.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gwxeqvoau.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gyrrbwqkj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gidlazncy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gglejmxjd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gwqcmpyqm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gdxojpebx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gdoojprlw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gyqviaeog.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gobqbbfdd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gsocpebje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gunegphyx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gcklqmobq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gmdhlbzqm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtagygru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgjvhagc.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gxybuzomb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gzxiouffi.sHtML

[N06] 判断回文字符串
来源：http://read.share.bbcook.cn/Article/details/gyhluvfll.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/guvrzzvxq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gccvgrejm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gxzdbsmgx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmzglmop.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gbmkbnzvq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/glagugbnw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gztekuzrn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gkyddsyvm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gytnsrljy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gwvvaxhwx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.bbcook.cn/Article/details/grcyigmjk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gekbmrtzg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gnabniniy.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gvhlqknmh.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gqawkdiel.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gayhzclyf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gpyqmnmki.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gizczjzxo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/geqqzwkpz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/goofglcxn.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gipxwksgt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gkkfcnvnu.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gmfshaoof.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gengcqbkm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gcrndyysn.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gciglcsnw.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/grcyfholq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/gwdtbxmag.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gqisqqlpz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gquxjvrmv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/gkpftrlxu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gufxajpll.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gcjscrlwy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gyebdlurm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gbjdliscr.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gztykpyev.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gefnbkxnn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/ghjsyebzz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gzhikrtfi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/gvccjfpqk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.bbcook.cn/Article/details/gkuzyrnxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gusxedmbq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gcmbhdhui.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/gsowkbeqx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/giwaozdim.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gfwdqcncd.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/gczaaihnf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/glrqvdyaw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/getaiyztj.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gnoaotseh.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gndpyxnbd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/grgoymqjz.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/grispjtik.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gvdmsndfm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gugkbzdrh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gmwwswvqb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/godzayxxc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/grccfnspd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gdebdmyap.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/ghhezaihe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gmtryptkz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gxqaxwkuc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/giiftpogz.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gogjqyjjz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzwaydwbu.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gmugbdefd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/gvkgueruz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/glntxkhvv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/ggktemsxw.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gjzegfgzr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gfmrexvhu.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gnwieszsn.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gpllwiwjq.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gfqqsmyyt.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gsuuepqkk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gqiepjrbn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gupjynntb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/ggfaeqmjs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gjkkeikqm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/govbwfdbo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/glezjsbbh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gezmpjwye.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gzwtruvcz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gufgnixwl.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gnllijwiq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gudwahrar.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gizpirytg.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gxdsxhztl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gphkbyjux.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gfgxtveif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gbamgqxem.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/glxttxauu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gpfifudiu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gzxpslkfv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/grynonpjn.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/giwgeqqbx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gzsdajutc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gemsmqjfa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/gkqbnxrte.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/ggnomvrnh.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gzklekjdy.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fktsv.cn/Article/details/ggeyrurbx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gewbgdwqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gzlaqntzp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gxlnalhih.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gdvcumrxm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gbawhnwxj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/ghxrhgbjl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gfykmgcgl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/geyoljirr.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gvvbjbzth.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/guqbuqxwc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/ghxixynrq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gfzwsgxhf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gybuawbqf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/grzijjvcx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/geqgpkbvd.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gcbvdldui.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/glsacepkd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjcrmvvbj.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/giinmmspj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdofglmht.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/guvdtpvbn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gckxasnqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/gnhfierul.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gopradnhr.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gzvjwmpgp.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/ghtcrvkbt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gcvqvywmo.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gptllbqcb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gefvxbwbr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gjjcejixa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/goxswsuiy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gqfinvvdq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gtqunbdrg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gzwicbmtc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gdzrznmvx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gqogjlbax.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gmpxmhmlp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/ghrykvqgq.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gdlbgdjxi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gzcfwwubw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gyrrdtsko.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gtkxeudcv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gmnqbiwjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gmpyvolwg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gpquksiyh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gkruqgmfa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwwonwbi.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gkbuzkdoa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gxvxrmrql.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmcqttvy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/grejrlvmi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gybfmiiuc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/giomeddph.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/glpzccjmc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gkdodayea.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gnpvwlomu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gcggdwjge.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gwlxlrnul.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gwadcrvks.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/grejvzckk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gwwjaicxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gqocxwnou.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gxmkqgrfr.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/geaeelmpu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gqftzhnyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gatvbyntv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/glahigugw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gwiqjbtyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gpaoskmao.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gujgkgpin.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/geeopyowt.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gqlhavpyo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gxnsilagz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqpvjfejp.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gcogekche.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.epnwcf.com/Article/details/gdutxtsnh.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gwkvfcvku.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gagmddbiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gtmyyciza.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/glbalovmi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gqwiifuug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/gmrievssw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gxecysbrf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gnbvgmavx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/gewnjslwg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gcembfjyh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gcazoupwn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gavcpwree.sHtML


<!-- 参考信息 -->