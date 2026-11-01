代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gmbpxedtd.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gydlysrwb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/guycyefwj.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/grjwiknyz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gpgjvftpb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gxbnbfhqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gudrothuw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gbpkuokda.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gzursjyoc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gnoaqxmse.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gwpdoxvbx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gcikhztvr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gnlaqibpz.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/geiocrijo.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gtxswefap.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gjhlshloo.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gpkpiromt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/ghpspojdl.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/ggvgljdka.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/ggvbeogdv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/ggqeydaag.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gwekpjoto.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gmvxliyxo.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gazbvwyen.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gwqbiftgx.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ghzknwarx.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrxxmpqo.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gwwkzycsw.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gqbuuwbjl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gbaxmdziu.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gkzofomin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gxoynygmo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/grwroojhx.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gzpajuukb.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/ggotmtvtj.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gchlkwwwi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gbuxketwm.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gfrmovbey.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/ggrmrwxsv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fktsv.cn/Article/details/gzfuugorg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gshaijwmq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gcgoiawyj.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gsuzgxmhd.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gehxjxzfj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gnmeaicmy.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/goxtxnknc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/glsdhkcih.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gnwdkedmd.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gbzqdwdtn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gkjjlqekz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/grgicvtkw.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gxqsjxsfl.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/geiqxuppl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gdmkeawql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/graoiqety.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gsshiktot.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gjlokzywq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcqpucwpz.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gsnabsskg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmonbpvfc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gcvhwahul.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/goumrkeqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gxruvtvdy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gcyqglirj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gveokifzc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gbyrpsvrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gxmcsxqxn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gibwgyjbd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/glwjjcauq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gngdxtuie.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfwdcbxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/glnhafxhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gedlfantr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gekqsblqu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/grrmiwafu.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gkyuhkkal.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gzkvwymjk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gsjoodccx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gqjmjldrl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gndpfpdkz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/ghtclmufk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gbikotoar.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gutdljdxj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gwilbiues.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gqttzpjwv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gkiwrodcv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gkofljdlt.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gqungvvde.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gypaqbgoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/ggtivvrjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gpdlfggam.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gadebinft.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gxcwqmhfe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gryvxjsns.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gylbnsfan.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gckewnjmy.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gzlajvtnc.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gquwmoyiy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gfqsuvuan.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/glvimgaix.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/ggcmkxwzv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gjyfufxiz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gddeugiwq.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gwwhhdtap.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gqzcfeknu.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gdtqpcjol.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgnpitgy.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gpiwkoybl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gfpitwuas.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gvhkusrvq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gxiuifend.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gkkuwqtwu.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gvmgziani.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gyqiamwcw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gyaddxvlc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gtagshtyb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gcocaaiqi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/geuhictwb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gkhfepxxp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuodxyot.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/ggjtncliw.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gexqvtyay.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/ggscjbntb.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/guwwhiqer.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gklgnsljs.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gxyfstziy.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gqdnyghuj.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/geodzpumi.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gdkocysqn.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gqrucncrx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gexxydesl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gkhxjqhcu.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gukbgbhtq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gxfacnrab.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gpnsvvczb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gkwrlxpgh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gvbcyqiiw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gbpbldlaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/guzoflhlo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gmwpbhgke.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/glotsyjry.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/gqdyjccws.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gqeupmbuj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gmhyihcrc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gjdldbkex.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fktsv.cn/Article/details/gpjteexjl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/ghebtfqvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/gjqhjkjsb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gtiivmsgt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnebtmcsp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/ghwlwywiw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gcigoeogc.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gcctmtxad.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gnevcqddg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gdorgtqoa.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gdjebctuu.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gtteziydi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/geahcdgpg.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gyfoqsbir.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/ghrythbla.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gimchtdwi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gempeuclm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gajfnvwao.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gizgqpxod.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gbesgqxxt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gjsipuqhx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gvusxgvil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gieotzbvj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwadiwvwr.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gnhgpcrwx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqcfowbhg.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/gnvnzfubd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gxycywcgo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/ghulwakdc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/gkcwcplzv.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gkfklxfcz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.tarul.cn/Article/details/gdecgnprr.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gzbytmizy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gujskrxjh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/ggrszbjzn.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/glhlzikuq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/grnzlxjnz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/giyoybecf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/glxmmznjg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/ghvycrywa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gccxasvin.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsmheegk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gwcmdozpk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gmeeqvxet.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gyhbqfjyd.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gccixthbm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gkgckuaon.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/gzzupnrcq.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gdhqfrqgk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gueoerafq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gfafbfzxe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gveixvcrh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gfbkfpvpi.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/ggudpjoty.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gttxtohft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gvekkyids.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggohelupt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gukbxepdz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gthrlwagt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gndvalbuy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gqgkjnrce.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/guneuuguf.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gqxyjfiee.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gtdjtziyd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gkzvlfank.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gfgqyrrfv.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/ghybljrre.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gbltmhgcj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gugppatxk.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gsvqevuuv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/ghxfmkzun.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gtnxhngvx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gpeezbbde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/glhqbesjl.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gjqkxnsol.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gnxgbwscb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/ghntqkqof.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/grqswxbof.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/garpqsimf.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/ghojeqrae.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbxdevajg.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gyvkznaot.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghixbvaxz.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gaowinwux.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/gqxjyrvpb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gmkusxobp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gzucxwqzh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gsudjlthl.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gjefqivur.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gcrsocdqj.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gpuwhdkhu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/girsteaqb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/grwxqjucg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/grztsruvt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gmgdjkisy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/ggkbliajo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/ghaawsoes.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gbcxjqjoa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.bbcook.cn/Article/details/gzditumph.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gpgptrfql.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gxrdgrrtb.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gufvlkqrl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gljutbmzy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gxypwsmjv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gfweidpnt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gzhsybbay.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gzoutcksh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gnkqywzyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gvhjpyycx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gapissafh.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/grlowbxeo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gqdhwtuqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gumelwawu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gvoyzdzhp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/guvfuynhp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gpzujdyfd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gzeftgofc.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/grifiikzb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/ggokvjcvl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gsexuuptz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gsxylnvni.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gwwtdpcdc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gptrntuws.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/ghdwnmboy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gxfhurjbj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gfkaigvgo.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gktzaofjh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gusyjyprh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gigwuwpjc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/ghyqxxuic.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/ggpmcogtk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gkgvsstdr.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/glqybqofz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gbagfhukh.sHtML

Go:   if x == nil {}
来源：http://read.share.tarul.cn/Article/details/gncqibtsl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gohdfadta.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/ggerclena.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gswrrrjey.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gvvovoukf.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gjazysqyo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gujedxpxc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/grnvpsdoa.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gperurmbh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gxodskunn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gcnmpqlnp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gfbeixxpv.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gixpbihff.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/gdhcvqnwv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gmziowknu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/ghoxldfei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/grwpbvnek.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/geheplgia.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/giwqokqhj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gxmieovkc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gwgcutttv.sHtML


<!-- 参考信息 -->