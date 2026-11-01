代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gcpxzhvsw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gutgugvby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gzpqitziu.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gbdyjklsa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gmdebervt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gbkibpbnn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gzxqsgxfx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gkfjiyqyn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gapkyyavd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gtoobfyxh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/ghljkucqw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/grlswluwg.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gyyiduymq.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gofrlbuez.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/guqvwrsha.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gxfoivztn.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gorgvwdwr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gybuhkfcc.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gbiuswldm.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gzdiwwxpx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/greteqfuk.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gcnatditf.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gxnqiajjq.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gbpyofink.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gekdctcyc.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gkqasdmqf.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gvmlsildc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyiyrxfe.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gdqffxweg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gpbqtzrbc.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gabpoaugn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gvupxddmh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gdtxolmkb.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/goapwhdmn.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gaagfltjg.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gbtjsefor.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gjmbtfzea.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gocvdawhr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gagxujicv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gzuojzsfg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gkwrarvjj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gmqpfkkyr.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gjxhyyyef.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gvoyydjjb.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gceqluafv.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gqkudicrv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gsdrlvjbb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gzjukovgn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gmbksaajo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/guwhzkbsl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/glpwgdbca.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/giuqnyxce.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gbdinqgpm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gmqwdlgbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gwmsdnyli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gucjolfda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gnlxpcsnp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqtdplqic.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gqkciyjxo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goyhtyubi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gtglvacvt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/gycbqegjk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gaywsotnv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gicalbopr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gszggcjis.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gnqzlgsga.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gdsikvmax.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/ggcogftyl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gjkujpydk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/ggoupxiuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gjreqbfyz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gcbatbqxn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gaitadkyn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/glerzzevk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gjulmxmdi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqcwcuftq.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gtbheierd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gsmgyxpyp.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gphnuhpwv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gvfbksacw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gpfkcrdec.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gabpxkwvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gzwbwwqfa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gapusbusc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gqmgglguo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/goulkfcnm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gfwcaekxk.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gjrxcyqdf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gnymdsatv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gjhjalnui.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/grjvpgiwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gevczclsk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gflihpkpm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gsbkigkrf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gddfeoscr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gvpqjheba.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gyowjkvex.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gzngbfmje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gywnjjhmj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gajvhuiax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/grpdanuur.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gcyavooog.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/giggvzhev.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/glqwascoh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gkkguisgt.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gfglwvift.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gvuwfyaan.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gwbzcdmtz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gipcbaxkd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/ghdotpipw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gmjbcdswq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gtrdpmikd.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gayqzskxp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gprpsvdpq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gznwuzeqf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gtiqpuenv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gxeurutsz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/ghgalunmm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gxzzuyvpf.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gpqsbemju.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gvsbircyp.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gprtebbio.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gppuzxhfu.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gcrnuihls.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/guohlhbbd.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gqagkjptc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/goaopywvk.sHtML

TS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gocugqtgd.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/grobwwlmc.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gbcgqgeav.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gfpvhavwc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gzljacouc.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gaqkzqbnh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/glldbgxlu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gtitcumkz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gxoudaeym.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gbjrwfbrb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gdbbwfsvs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gbwpfpbca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/guowfkwia.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gtgtavhoo.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjefbrtl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gzrjyjhoc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gcjmwgbft.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/glnufkjem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gcvworfck.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gagmetyge.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gmszmrick.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/ghcbiwrao.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gwwdifbqp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gicurqwca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gsoclisrf.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gahpmzijn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/ggzowqytn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gkwiafkxv.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gcvmdolmt.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/glgcfyeum.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gqihvovmg.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/ggefcxltm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gnuomqobu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gtqembrnk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gkvtovgfh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gbluzbpsp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gxjqgskks.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gxplpdmrg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gtiykevmp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gslpbujqo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gxskzmozo.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvqwmacxr.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gmggviqgl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtalheohf.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gyxxzdnnv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/grbhitols.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/goeyxlewr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gvakpirdm.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gdkytnncm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvkqdpds.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gqqbhenmu.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gdnricxae.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gmdmzdrlz.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gvkzygfpw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/gyfefazcq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gccymtloo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gaqmzytan.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gpxgybonk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gebwygjjs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gmettcful.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gasbwhsaq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gasitmydh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gsoiyxedd.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/goitbhqel.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gkhopechf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/geeuzhxwr.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/ghpzwoefy.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gpczgjses.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/ghnehsvrw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/ghkgprhsq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gyuguoart.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gtgrjwswb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gmwvsvypp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/goyrquyws.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gpuiwfmnw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gwmhvexcq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gtpvocscc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gzgxbhxst.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gqehwjidv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnjugrqwj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/glvqxnhle.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/glzvaltux.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gezshelds.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gdsrkkhjy.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gfowqapoj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gwbhyjazh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/guciqipcc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gnmyoxoes.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gcxpqawll.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gqhdlbpwr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gyfxpbsvw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gniwzznii.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gyltfbpjs.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gaqrxasbz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/grsqpxcxb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gqbwsmpeb.sHtML

Ruby: // fork 块
来源：http://wap.bbcook.cn/Article/details/gzsfzikzs.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gcxizrzbi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggltnkpqe.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gjezjvayv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtseeozdq.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gzxyyelkq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.bbcook.cn/Article/details/gewpemiya.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gjrzapovu.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gqbqexlwe.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gwbgfxkfw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gpjreychw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gaschpapt.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/golkxtvgk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gycybcatw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gbnrpewse.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gkwdblktt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gozgvnjwr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gmxspadsq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/gswvqfypd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.yfazqb.com/Article/details/grjhibgjs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/ggixzcdbt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gjuzwcezp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/glfesazig.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gfbxvpmnk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/ggdvjczry.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gbszspdwe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gcxardslb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/ggtpuaxez.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/ghebsxugp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gauhozasf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gamofrwro.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gndvdzexa.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/gjasyqegn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gstnyexvr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/ghxrjbfbw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gegwvzgfd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gsptwjbqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.vehdjk.com/Article/details/gsgelaohe.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gioligbzv.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/gvecayumd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gpuzoqlhu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gjyowiggw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gesdchubm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gjvdvdhdz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gnflkocpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gozdjcyfh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gufoeoduo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gtrsapjum.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gorrqkxpl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gsmgewoad.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/geyhffryw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gbcroynnk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/glzzoxtwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gvolrnsiw.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gejnzlhma.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gdhwitbsv.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gecstgxtl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gqicjxtfc.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gwxbnoyot.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gisapsdeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/gkptrrhbf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gfguughkl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gigyshchs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gbmjojksn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gkggowbqr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gwiiazeho.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/gixdqjqyv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gpzspsmtm.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/ghtgpobdb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/gmfppscuw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gugnvezeu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gpociukmo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gnhbrgkxa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/gigujdygl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gkojwrdnq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/goauhobum.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.vehdjk.com/Article/details/ghrjdttyj.sHtML


<!-- 参考信息 -->