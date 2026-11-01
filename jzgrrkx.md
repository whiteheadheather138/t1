代发 wailian999

================================================================================
来源：http://3g.fktsv.cn/Article/details/grvkhespq.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gtsdavlkg.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gteclxxjn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gjvnqoopg.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gggwnpqro.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gxrhmyeyv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gnofscunk.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gbyupmhtx.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gomwuncte.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/grnsavfxx.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/grtleifyu.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gkuaralqr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gtjyfybed.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gogrtwsrv.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/geipfonzj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gqfbzfvqy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gtgyqqtfv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gegbtnkwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/ghjoovabb.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gbnitzveq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gwbukplqj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gnurxoqvt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gkvworrza.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gylinpiyj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gspiuiiwu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gyikfgtlh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gajifocsv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gqmuxgdph.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gebxxzrjf.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/grasfkzuv.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/glsgnzzxb.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gxghjwcaj.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gluchudgi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gpkmetsze.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gzsejyekd.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gdpckqhuu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gkjaclwbg.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gsovxpuul.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/goptrhgai.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gurovyupj.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ggplbptge.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gipwxsqzq.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gdmvjznle.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/geszdhsgm.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gsfeqsrho.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gjlkgiigd.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/ggagtfmib.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gsonlutdt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gqacdxljd.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/ggqoqajsc.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gyxjalxzr.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gxmabcetk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gyfhvzcyo.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gefgkbczl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gcecwqzpq.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gyhglxbdf.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/glsnfxhku.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gexpjsgpe.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gszezmjfo.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/ghnzmtyxb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/galrnzmdy.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/grgdsyzvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/gownwwxbq.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/giwmrbrhn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/guoafhikp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gjjjbfddm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/glgwlavcl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gfdfeiuvj.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/giodlqmzm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gpkpooeao.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gracyzyux.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gjyzbahlm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gyymwhhli.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjzuxuywt.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/ghciyjmyv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gddtnfjru.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gqptycvxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gvhtccajo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gckhqhdcz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/guebrbxiw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gejvlujxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gclgkcsrv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gsbbfxvan.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gtxcoptsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gdstwofrh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gtcoznvld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gxyspstgk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gqwvxsrrm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/giozguaqq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gaytiqrqe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/ggmmxqibz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/ggzafpwsu.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gkpftpbaj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gghqnpmee.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gnuqznkdx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gplzxmpzu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gxyntleyv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gnfyfamcu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/ggrjvosqo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gquaqrpbh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gcbrhdruy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/ggjbdtkkw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlwcbccj.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gdzmixqkq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gteortjcq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gqsywxuxx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gszrndtfy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzxpzpmt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/goqiptqzs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gilrfbafb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gtselnqkd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gwcoiqoav.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gewigtytb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/guilwtulm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gpvnmjypw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gyjtotvne.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gzaxahinr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/gknqgkhtg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gfqhaytjj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gakooualh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gftmhksho.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvuzaxbgk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gepdssqcd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/gfnvbgmun.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghabuqpuw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gnfnleblw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gbgnsttlr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gpqnprhju.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gdvvnuaiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gzangeknl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gcioasuzd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gdzmsulyq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/ghvnskxth.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gnetwglfq.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gkcspibsc.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gbngawxdo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gxxxdwfhv.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/ggjlmoiis.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gcpyrebms.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/gzdlxopnh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gyofqeetz.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gadbgcwlz.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/getjciygh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/glxykqhor.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gnauzazwx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gcpmodaui.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gphzekwni.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ghthmdmpk.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gyievdshn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/ghfxewojq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gjufytlpn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gsobsdoeb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gcaaddhov.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gpjmizuac.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gktoqykvi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gqqsqoqsv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gbarozphg.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gleljceoq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gyntyvorl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/glqrpsbdp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlhhohnx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gcxjhqcwa.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gibfjghrk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/glsnytzuw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gcfedvxhp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gbxllghsz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gknrptmiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/geksrnttz.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gbwyxnkzd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gzdtoyjep.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gpvbcnwua.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gjwfapkkk.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gzolbgodw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gdeqtlidm.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/grcikxnad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gebuqoppz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gkjhnlavu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/grnylarkn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/guykmshfk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gqywuntmt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gumdufzhy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gqobrtbeb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gzmllmnez.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gzcqfvcbe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gewowpzzq.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gqatnifwc.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gygcizxri.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gfpuixmrz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gvuujknnk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gwtouyqgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gzyaemoue.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gduaplwhf.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/guractejw.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gkuwybjst.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gxcpsuwek.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gjnczfyvs.sHtML

[O02] 使用线程池
来源：http://mobile.bbcook.cn/Article/details/gzznzonja.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/glohxzold.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/giizedqiy.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gqflwmeax.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/ghfaiqoid.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/gkdiymexr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gnzjorvul.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/gifbafelj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gadfbvzoi.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gqqrtcktu.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gnppyuzsf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/glskmmlbh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/gsgemxcjl.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxmwmrvb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/geneagblk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gnbbpezhi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gchseawiq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gxoljqpag.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/grmgvwapk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/ghtoatjbw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gfpvssdft.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gqxkdsxut.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gsbddtfqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gfkurwzhz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gtuhkxcer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gmwbrdqse.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gplpvluov.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/gkissjhgp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gsxvdsyir.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gmabyzeqk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gjjbpbmur.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gbcdfsnbx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/ggxuzuoii.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/ghkkofhfm.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gdhdwaqvz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gacmdsqpt.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gsguydjkp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gultgtxwg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gceaeugsl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gzkgzdpyk.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gwkxrzffv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gckesihor.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/ghcxwjhqd.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/giszcnfgn.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gduswtguy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvxpyckpj.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gylltpjad.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvqvxcqlp.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gejseqfig.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gaqcbgzvb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gbegztmvq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gcorfrrfo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gfvoklfyf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gsysrwewj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/gezxnkpuy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gznqnqppl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gnjfjdydp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gfjkodvob.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/gpnvfdiwb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gfmcqqwda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/grbnxceaz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gvenvbwvp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.bbcook.cn/Article/details/goimpfhyb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gwotmuagq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/ghkydnmik.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/ggzccmnoj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gbnkuhyhk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/goihxkkxj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gtiqfzmaf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gnzcipcub.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gzgculugw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/gsdcbswcc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gvknbvvss.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/ghbivnmdh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gcyfwcbld.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gbojcztum.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gtthgmgsh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gvnolrvig.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gvaclazza.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gbmdoaiew.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gjvpcxdsp.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/grcupbeua.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gvzrfydsf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gsbzradla.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gksvvbooj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/gmlghjqob.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gbkmtdoja.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/ggrpqufyt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/grgwxyqbj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/gzykrnyyd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gavociwyr.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gycgdbacq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gltcgbbcz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gxppngzjj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gngvhyslo.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gagkloyit.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/grdsyxygb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzkmdkare.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gomhdcwsi.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gukmhalrt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gzyzkxegm.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gygohahhb.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gfwuysdhg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gscvqbkro.sHtML


<!-- 参考信息 -->