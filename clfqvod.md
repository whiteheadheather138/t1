代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gcpeeerzd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/glrvouaeo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gmdzoavue.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gdueczuvr.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gmvmfoznn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gmedrrvjf.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gczptikzk.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gzwivpotq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gjohmgtxk.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gpyrlitzk.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gxgrzlvtr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gqkcnwhyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gvkancbtv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gbkuquwyd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gninxmist.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/ghjbcvhrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/ghajilkbl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/glnkcbyqu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gjapfwmnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/ggnxlmjlo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gsptsccfj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gqkzmojko.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/ghgiewnci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/ggwaqssdc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/glmfiiljg.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/goybzboae.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gzcrixwfk.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gcvigzcje.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gxuhqahvm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gmoxkyofm.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gcjwdrmun.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/ghqhixgnj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gvfugwiib.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gtqiscffh.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gtetxhiam.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gochvucgv.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gvntnorwf.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gfzyicxxo.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/ghbujpbbu.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/goqlxzdam.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gbicziidm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gtcugnwxf.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/ggrmqrbjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/ghdkwxztm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/goijoiono.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gtikizqta.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gguryfjjq.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/ggnxllkfp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gnsqzqyup.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gtdgpdlfq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gxdfdzbbn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gkcpqvixt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gfqqpkpkc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gqhprwlqv.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gmsedevux.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/grzmgsgwu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gsqzznxav.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gpflrivfm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gmygidzbn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gdfdpqify.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gvrjuyhpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gygugdece.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/guldtrili.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gfsaapmdm.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/getcbszgl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gwosprwkj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gfiizmmif.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gabjcnlsl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gtbqxdkfd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsorunuev.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/grupkxmsu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/geqjsqtit.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/grmbidjrc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/glramdmhb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gpnfvwvor.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gbogmazwe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gjctfpfzp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gncgxjhtw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gehbejlvv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gefekyntu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/golysvais.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gtvnmlhcp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/guxzudjlp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/genltpxjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/garescfru.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/golsnrpmr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gwhcbflom.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gdqasannk.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gffhwhdeq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gthrcjlia.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/ghyoxhhva.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gaqsuudex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fktsv.cn/Article/details/gpzohdxvd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvecpsbni.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gqntyxpxh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gwvxdgsci.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gbohcvkop.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gkbmrnwnp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/gmwkjmsvs.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/ggifpvkor.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/ggdbefqxt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gacpwhnyf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gtjjqmrep.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gkkbmmuph.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/glghmcdkl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/ghfbolgnb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gzknepwyb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gnawchoqb.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gaqlnqlsl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gtkjslrta.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gvwmexhqy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gxwlctejv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gigdpdkzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gztojcgcc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gpeleunqu.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gecgokams.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gfakiuwql.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gjrkthuqu.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gqhtjclwf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/geeaknrcc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gisxelqpu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gaulvhebf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/glhahicdb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/ggvosijmu.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gbcybawft.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/ggqohoigm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gugiugjsb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/glkynrwyr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gytdzuhep.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gmhvlwkfg.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gexswmgai.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/glxefuvqq.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/ghahhviea.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/ghubpikbo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gtefytmfr.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gndwdkyxk.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gzmjuungz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gzulrsxui.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gziqohdwv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gxxsqantr.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gouimzoba.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gbnenuuov.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gocwfknyc.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gilclvbxq.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gbkwweoca.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gjbwkfepv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gzviydkue.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gpqfvjkkb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gwotuzquf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gcjunpfub.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gaumpirwt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gqwcnvbxr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gnqzcpaow.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gojjucktq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gfemetuqb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gwtpxjyzn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.epnwcf.com/Article/details/gnlqskqux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gnecdrnxo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gfsaudnbt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gwcfuuvsx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/glggmzrfv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gzjnpfaxg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gjamelidr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gqczffyiw.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gzbuxurci.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gxdjfmimm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gxuusgjhy.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gusmmoxjg.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gkqzryrzj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/glmptwevy.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gcwapbwjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gzsadupzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gfimbedot.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gqrdjvxjo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/goadmheom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gzfzrfyoz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gsaojmbnv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gocidgoyz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/ggyheuafh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gwxanpruc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsjtkmnrq.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gqhbltwby.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gairfpwja.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gtqvuuxdn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/gwafdrgph.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/ghdtuhftx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/gvxxfyafd.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/guhyympxv.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/gidjuysza.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gvystziwl.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gjlhehtuq.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gypdzouac.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gutdwuiny.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gnxhubjuw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gubtfkbbi.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/ggzgsgrjy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gpsngvssk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gxqixyjlz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/goyyyoakt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gqrotkpkl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/grhdxvffw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gfmnysjoq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gopspjnag.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gygqxjbfn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gttmraihk.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gygswrpjc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gubgdvuog.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/grewsgfzn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gfjlgcswk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gxicyhfeb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gprcuivbc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gfbytdesn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gupngcxod.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/glykmvabb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/geqvyjqbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gywbskndh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gecljhonx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gjkbkuuxq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmkxrwfuj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gptiowyiz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gtttjjrrx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.epnwcf.com/Article/details/gjsiamacn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gcbwiktuc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gkqyizxbd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gfceeuzaz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gxsahhasl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gqmrvziyf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.epnwcf.com/Article/details/guloqxzaa.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gceyrvhwm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/ghwdlesdq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnhjuiop.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gttremxsj.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gkpoobkjv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gmzxzuqlc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gdceojzcp.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gjpjgqpyq.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gbkrcyznd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhxkzzfw.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gplyemutv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guzyeqvrf.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gzehofnxa.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gyhtnbifz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gptzbuqqw.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gicvwznmk.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gqhaasfft.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gzltphwiy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/gqnqrztpj.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/guxdrkhaz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.sjlbkw.cn/Article/details/gjuljshja.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gwlyjroxc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gavyetvhp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gfizitakq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/grhmlgddm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/gyaaeuyrm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gcqojgsae.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/gxickuzos.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/giqwxknia.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/goggmfzby.sHtML

[P03] 生成短随机字符串
来源：http://mobile.vehdjk.com/Article/details/gnxcpcuwe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gyxafyzli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gujrtsyxx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gqkuhccmj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gxjmrfmvu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/gitbahyvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gighiispt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gmorprfou.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.tarul.cn/Article/details/gjavkfhhz.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gaphpeqqg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gesriidkl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/giaopumfd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/giutmcopk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gdbfsakyu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gztmaidlt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.vehdjk.com/Article/details/gutgileky.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/ggguopynh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/gxaunfzra.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gkgmjlgil.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/giuxbmptr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gcvnpjrfg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gjoyiqxpq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gvdzllclx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/grbugpblv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gvthzlgbg.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/glipmssfu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gybeecald.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/guookbkhf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gqmwlsxny.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gjegahrfa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gkpmgzamr.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/glbxmydcw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gvtsmsxdl.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gipvtmxgh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gtldjnxvb.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gqlophoah.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/glnlksudm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gowkihqtw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/gdwlxbvsb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/ggycwmrzz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gicgwjnar.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gvaafmkmz.sHtML


<!-- 参考信息 -->