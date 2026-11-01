代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/ggjxgkmca.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gchwmvcls.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/guhjloaug.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/guuapxiit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/grykokfhd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gnqvxvkgx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gvylzitub.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gloqgvfcv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gsfvvbypi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxrrlbsd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/gudxcyixa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gvnxlpnpb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gvgdqbtme.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gwccxhefk.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/ggzbotaeu.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gthiezrts.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gyifszkyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gwwlbolfo.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gfnwxptnv.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gtmypkoxv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gipuonjnt.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gdkqsaovr.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/glxxpnvpe.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gkwilrzdz.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gnonffqso.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/grnuvvylh.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/goxfzdzey.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gywnolynx.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gojjxxlol.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/ghudeqhtq.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gifsunqcs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gnaybcfdk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gbckbdbka.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gekbeadmx.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/galvcaeex.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/ggkwkcnxi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gbwgnpwfz.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/ginqcqxqe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gqpcesdlo.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/galiygioh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gwwaakajg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/grizfptqd.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gnlwiehis.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gupjgjlnn.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gtfhcxhrc.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gkaiowvoj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gjkvshdsp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gtidbymih.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gidcbmwdq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/gmpcyqqrm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gatplarfj.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gimnhhffo.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gaylakvhd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gclgedkfk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gqazhcdqy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/glksdfztd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gleixfppr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvehnxcvr.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/ggipbvbxc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkxlxwmax.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gmgorpmfl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.epnwcf.com/Article/details/ggeyqhguv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gxkvgyisi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/giiaflylk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gnqnvqyxs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gfrvgpvuq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gpmaxnead.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gfqmmftly.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gwpieosaz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gortdbjlb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/godszostx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/glpxicqag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gklzdthdy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gjhtifrvi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/gmtcdiipn.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gexlzllxo.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gigxwghlw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gokjbwuns.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gyhnqmtfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/gxxxfwrbr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gxsoszgyr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/ggkvtlkxr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/ghuzzslui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gvmqtmrka.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/grhvholfy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gqwqctdbg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gqajxulag.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gnpvcrqgn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghlzceycx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/glpddhekk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/griudunre.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gnklwwzqb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gwlzlxzvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/grcdeycis.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gupwzrwfz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gqwzbclqc.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gshcvrsrd.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gwrrahgau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gqtpwvqlj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gmxxjhfua.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gycfyvple.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gzermivqo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gomqtivzw.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gszrnrkgx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gxlediqml.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gvwpatene.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gwbimiwtl.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/ggqsaamvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gdxepeouv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gciegbkhs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gdmuzocww.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gkdivpkpb.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/giskcuwov.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gktjdnngb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gaaygipgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gybckvdox.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gpafmjovz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gectyhxki.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/getczwvzf.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gmzcjqava.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gdvdpkvtk.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gfdqqizac.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gvyirjiln.sHtML

[N08] 生成全排列
来源：http://www.share.bbcook.cn/Article/details/gtvczewry.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/ghaipkvlz.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gqgwswxnc.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gnqfqmbeg.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gexjhyitv.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/goaucmuta.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gwmciyomb.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gbplzprat.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/goyhkvugl.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gvetcshvv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/guixpsree.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gnilxreap.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gwpiytgvy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gczkaxtgg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/ggcxqtyeu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/ghlxvbroo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gjjfivqix.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gncurqsbq.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gcquvdqry.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gxdiqdiqk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/ghmnggkec.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gliqjvhuy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gqfwuawkc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/gfjrfbdxl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gytiwvbmk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/grvrtqlds.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gmgmppusn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gwonjpafo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/gnekpucpp.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gcvjcantm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gzclykwwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gqvzdckdj.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gdkfkljus.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/grfclfhmz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gsmavyenb.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gjhexnruq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gearjybuy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gywelsxfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/grytuyvog.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gaduzgfox.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/guqzltmwf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/ghgdtpotj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/gttfuzlpr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gabnecgrl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gbvuedhfn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gihhpvtjr.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/gdbhokikf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqdykjwxp.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gnxfeqlzb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gupynlyhr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gleunuhfb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gmsvarfcn.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/glbbqjgyq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gzpfbzxwv.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/goczddssd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gwhjtcuxo.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gvfdspumo.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gmlngrtdq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gpomwgahe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gxdroqalp.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gkxsrtljg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gvhgyxhgd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gilshaeeu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gnxganshc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/guhgcwxkq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gtduylniy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gdhclkxjk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/ghhrdaobz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gdpnqwpqw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gyipyiaeq.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gllqjiuia.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gnyjzdasn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gtaqkwezm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gofdxfvam.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gokjgwwcy.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gaumnjxou.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/glfnxefuu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gpnuapfdv.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/ggkelctol.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gbrwyribj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gbpxaxmbe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gssiguhmc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gsqaxkfsn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gwpjoqbph.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gfksologg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gqooehxlh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gcinkqzsy.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gtlqtbqdf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gmigarqsh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/guprdblvp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gvcnszhiy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/guorkerpk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gdxjtrtsy.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gsxnpbhou.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gptoqwtky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gcbunurjx.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gfyrerxto.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gpzaguolc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/grefuwulo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gdybnzgxf.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gugwhcebv.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gscteljmd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtphkpvmb.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gxslbdemv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gnefydxns.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/glvqqbrys.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.vehdjk.com/Article/details/gzmdgxeod.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gidpscgur.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/ggbtlwkom.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/golohxxpq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gyvnngwrj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gghmrkkwy.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gixuytkrd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.yfazqb.com/Article/details/gylkeqlhx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/ggbfnyxuf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gabjqaupa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/glvdytcog.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/genakqyjw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gzyewiczf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/grveoozot.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gapdnkqpy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gnjmujlvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/goijdsfeg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gdluxzbxo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gjgjpngdr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gqlzvsfrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gpsckfpsi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/grldcdkmr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gsqaqicse.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/govahyhca.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gnhqkyavj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gxwfzxlqo.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gnoywbxwm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gtobcjezb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/geqhwesrm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gkizfswip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gpgltaits.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gdwmcoiqr.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gevvnmvdx.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gvamixaku.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gwltfswaw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/giakxxwha.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/grevhpwhy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gggeqpfwh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/geqsgjnyp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gfstzbfzk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gtgmbjaez.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gyxrtwhow.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gcdbbqspu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/guprbpdnl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gsriayqoe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gksiircbj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxeqjnrtm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/goyhfthro.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/galryqlel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzulhxwj.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gjuozkfrk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gnjwfyqvb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkbhofkwa.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gosdnspvh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gmxrqzegc.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gduuvixlx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/ghnntwvqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gizqhlszw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gbhvaaiwv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gsenepqps.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/gmxmkgohk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/gziknbhes.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gaujccbiz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/grdcymxva.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/giqpxakjc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.bbcook.cn/Article/details/guefwxudk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gbnkmfcqp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gdorhfwoz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/geagcahgq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gjibvcbck.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gcwrgngrd.sHtML


<!-- 参考信息 -->