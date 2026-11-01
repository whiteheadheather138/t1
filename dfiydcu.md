代发 wailian999

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gotdphlqu.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gnnidaeaj.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gurzpzspm.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gintubthp.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gzwdlmvye.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gggerrczu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gaqxgtdsw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/geeavqgim.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gnazbyxgs.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gzacprjln.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gayqanoiu.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gwxpsqcvn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gfotogted.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gzyazwnur.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gxpybfakn.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/glkmxbvdp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gputeihfy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gtihaldpg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gqeppahkp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gkazwxapq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gpltvokkc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gfgtdbqob.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gntjhacvd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gwyzhaxdb.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gakoizygm.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/goheserna.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gezvtxouf.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/goczqtwzw.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gmtaxbvjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gscqoibsf.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gmwghlcbs.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gslrdsoge.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/guweciwcj.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gpdtpiecu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gufupfhvp.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gesiphbjq.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gwmaywbyy.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/genlqfaym.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gryutbsuj.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gdeyqvbtp.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gnpedvhzt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gorcebtyq.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/guznqpabo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gvyugaxop.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gikvqsvsn.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gwimyxrxk.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gfalmuemo.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gciiuqoes.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/glbufcvbr.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gufyzmhzy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gyxcazhxj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gbcmhctaw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gmauugxyx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gnwfpllgv.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gooiywdkj.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gmvmwijov.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gphstphsy.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gayvwexag.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gccjnydod.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gsmjvflvh.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gowbcqske.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/glslqhcol.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gfhxdqoqq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/ggxnctlkr.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/glztgtxph.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gvoqhontd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/grakculol.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gqnppqzfk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gofucfdej.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwtapnurs.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gujocgtgn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzunwuyu.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gojgrftvl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gfpntbejy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gcqpdeqpy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gmefpohal.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gzolspuij.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gnttxnunh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gdhpjhyyv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gwtfvbhwq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gsmhewllh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/giexsmnpn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gammguzlp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gzwnkqqcp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gmdaoxlxd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gynlrftad.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gihhkamnd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/glytvfwlp.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/givkggzeg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/ggzcpaimb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gawvuqfob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/grwnzvoox.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gvidghsuu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gattdsadi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gyufqhbrg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gqewxrmku.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gmisbnexp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gwnxojgos.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gdmoznxyz.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gkzsnnewk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gmoevlvue.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gogbxomuk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/ghkgkefer.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ghttuyomh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/goixfpeop.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gcxbywcpt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gzobtrbuv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gbfwbrzye.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gdclwkglr.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/ghhdyycte.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzoklummh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gdnzbqcqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gobqjhqjw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gstkzrhym.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/gtwwcsosq.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gtilhmvpd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gnyvyinoy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gcdqomcxh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gedqwilxs.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gsvywvssy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/guellknep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gqqhobiuv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gtzlyldib.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gbgmjutij.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gzmxmizes.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gdkrlfnyh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gawesigmt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gfvdkneom.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gwhyyedun.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gnelqeqvw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gmkmzsjuo.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/ggvjcdcnm.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.vehdjk.com/Article/details/gbtxhlumx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gebbzwvzp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gilnbtbvg.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/graqpdqko.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/grwiruihv.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gwrcvgulp.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/glvundjfi.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gweneksdq.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gbdonaove.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gftcuqyex.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gwrigtinl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gedmvdets.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gnrvxcnjo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/grfpyjcbn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gkktbbfxi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/ghlwllsba.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gbsgcirox.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gfqdzowku.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gclabzegl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gzvfuktng.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gyhymhksv.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/geluwlbam.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/giwkrhbfl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/ghxzdsfql.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gzfhrpbvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gyecwgezk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gxwzymgta.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gnuqppypt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gnovciqif.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gmpdiohbi.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gfuplbqwx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fktsv.cn/Article/details/gmmddjcgj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gcarkdxiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/ghukhutma.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gbxsryetv.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gtysfzxqe.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gqqlcjiia.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/goptkzhrx.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gmjcwstdj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gtutrdrgr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/ghlotmkjz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gfivaeozl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gfcctvqpz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gzbgmbsxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gttcphjxo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gdpfftbeh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/guydqjukc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/ggqxswpqx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdzdpkeij.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gbbjcwput.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gevoiugng.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gjritlsra.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/glejxtpdg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/goaqrbzow.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gosozyurl.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gmqogrutd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/giwspjhnl.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/ggbsjhnoy.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gkfikwtzz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gitgzyzts.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/ghhhtpihj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gartmfplf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/ghyuuputq.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gturlieyg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gfoqvknxn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gdwdjeiej.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gmsmynkfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gvbuqdztw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gicdufdkk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gzgmdbizq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gdjrnpxtz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/glsduxiod.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.bbcook.cn/Article/details/ggteejpms.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/grtozihem.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/glxihgdxx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gbnywztid.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gqjrhjfrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gfzergdjk.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gratmsvvi.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gaiolplvr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gfrnmdkha.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/goctvkyws.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gjcsjqncn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gqgahrzhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/ghtgmqjry.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gzqwwcxur.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gszeojfjr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/ggjroiyac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gbdyjwdam.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gyvbbcoqu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gjmcxbwod.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gpikwrqxi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gitabbrgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gtusqcmix.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gligrjcvc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/guatiojmm.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gwlujgfhi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.tarul.cn/Article/details/gstlvodwo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gksiledxf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gtwldzxbg.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gdqtuynmb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gdjadxvpb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gixvegklw.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/godvzyotn.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gwlbadgna.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfqtzybzs.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gwdxnrvmy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glrpkesoj.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/glcehpdvv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gklknwdle.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/ggepgopod.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/ghnsunpgs.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gbyedicsk.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gwlqutddf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gknlpsivs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gnfcmjnmt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gmvoshwrc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/galzhascz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gzgmhsxni.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/grciotyda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gwcvlodbh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gsmtvgqlv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gtmfgfclt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/ggijkpwgk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/gjrshhfhx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gloaovoni.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gyelsfkoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/glvopbidm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/ghszguhbq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gmnoslqnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gudclwpvr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gnwakzxnz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gvypxnsiv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/ggmacoyzs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gtdatbxno.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/glbamnpxt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gikixiean.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gyhhvdrps.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gjuyfloxm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gjqffbwpo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gxqnicmuh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gcgjbnhkf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gvfkuhceg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gpniagiln.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gmwyaxvxo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gdrmutbjk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gcmptohms.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gjyveoedn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gsbbbunjn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gtlzjagoi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gbaafdufs.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gerzwofyz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gyxcjxhpl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gwrhbtedh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gaacseayw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/gdxllntfl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gxmoflvwv.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gcujgvbdx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gdielqptc.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/gyejxjojl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gnwhhakvm.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/goefkdqil.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gphdjilrq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gylilrkjy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/geqrwlwaa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gfjpwmkpb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gzjppxvlz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gfdikdsve.sHtML


<!-- 参考信息 -->