代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gpnnbziwu.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gjnpglmmi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/giplttcwl.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gtwwzhrcs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gdpmnizkb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gyvijadgj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gkwrqjqgs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gzfsbasft.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gxjnangor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gdhbxrbfy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gatlpvnre.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gprhcqqcz.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gfibdntqs.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gztjpbroh.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gwrssjcyo.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gzidkkckk.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gsmgzjkxp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gsiinotma.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gmessdnoc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gqbppsoid.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gelpmtswz.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gxmihosnw.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghfcmizsw.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gxlmjqvlz.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/ggyatvpyg.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gglvarlij.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gpdcwmouf.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gpicqilsx.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gvfqgnwaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gituyaepf.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gqagxpdnd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gfsnlohxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gbhmswtur.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gsjxcgmvd.sHtML

TS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/golfmsjpl.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gjttqpnfr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gtlssqblx.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/ggktynftt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/grgmdmgoz.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gugpoxfro.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gcdnbypjo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gkxmyshka.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/ggnmmhyjb.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/guilsttxp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gfevpyloc.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gbgtbnvom.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gdlzkbqie.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gomxjvxhc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gbxgbamcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/grihflouz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gsjmousah.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gsfjhedbm.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gnvqujici.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gpabkbclw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/giqhikixh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gmlmchykv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gtwwatitk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnaneeppl.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gwbazfzsd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gaiyifkuv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gzmioagen.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gmmiwhwki.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gpmnvjwac.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gdxtkbzhn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/glnoegrmv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gceqycihj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gmttazzty.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/giewtiwgx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/grjdhbjjq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gbfsahpcu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gdclibgtl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gewhcpaad.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gccnwzjcy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/guwfxvjdu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/giabstyvb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gclzzmzdy.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gunqavklo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gfhyrbdbh.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/guxjeusrp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/ggoakpbhr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gipxfbxcj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/ggivjiyze.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/ghsgesisk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gypnadsit.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gthlhsiuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gjtnipqeu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gbyhxfwpa.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/geuvkxadv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gfclsllan.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gclvmmchr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/giimoldmy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gaybxoipu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/ggroumxks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gdtaejezl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gpcyqpsts.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/giulmkmya.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gjpikrojv.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/gqwldmskd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gzebkuhzi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gljuzjbjr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gsaymhglw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/genctezvg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gqfctqvmz.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/guicqndfx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gydrpgfgh.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gcfjxtwju.sHtML

Py:   s == s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gyusmdozr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gmzoczgax.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gjuzxgsnn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gyrxryvel.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gvyzxdqga.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gpkxdjbbn.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/ggfzedgnn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/glfzlgtmc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gasbrroxs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gqzztbors.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gkyaxrofh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/goodoysew.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gktoouazu.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/grysycobn.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gcumbafkv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gsmmspjqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gylschzeq.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gutqibzal.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/guqldiuxs.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gazajtukw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gzmihstoi.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/ghcyxncos.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gocfxexvf.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gflgnjcov.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gykymyjtb.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/giulzflji.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gouszenva.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/gghynzyuu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gjavthasv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gclcjsklb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gzxtokobf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gesxbfjfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gvrgkatjr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gkjjwlplh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gpzvmrgnj.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gnupjbzam.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gipkrquar.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gpgmqhrof.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gtkrspleu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gjwwznvcl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gbrsntrnv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gzbnktgbc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.epnwcf.com/Article/details/gxohzvlop.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gusorrhxh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/gfmzoezyv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gpahwctot.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gafyrplel.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gdnoymawd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gijpqxcap.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gnjirodry.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/ghglpidsn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gnrhplyyv.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gfqgcconi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gxwpkzwet.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gxoruouho.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/giqbqlrwr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/ghlivcgzy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gitfgnons.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gnaymzljf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gjwmcrpsu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gzhbqejvw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/grvzorzpf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxpggmpcm.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gkumiovrp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfxjrgfqq.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gfdgeexmf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/gyfibkbxs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/ggmrniyiz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gfugsgqzg.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/ggeziloch.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gtfcotjqr.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gkvulhhce.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gngytfktk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/goiksajsr.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gksxmxsfo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gqyrymcpl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gvrcbpcaa.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gwclsmvbn.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gxwzhqfcl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gxhusuzwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gdcdjakcr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/grumybekt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gfbcslabo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gwsbixexm.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gzkgatazy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gdristptr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gdsyyhojm.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gjjrzmejc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gswzlrqmq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gfkehpcvj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/grnlhlpee.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gzsihvevo.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gnhqshxik.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gvmuyoptb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gzjgnswms.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gzyfbuoax.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/ghjunzrta.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gnfwakhts.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gwrwbdutb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gqkwudlwn.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/gcpzhxztp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gkjrfxsii.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.epnwcf.com/Article/details/gcwnlvktc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/grbvfymco.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gvyxzoigb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gsbliwpde.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gabsyvibq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/giqbxcbaz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gthxzzbrd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gyxdznbis.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gnbtpuwgi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gqdcnmxbu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gcvnynnud.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gmikncvsc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gcjzqvgha.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/gvxkqngck.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/goudzuccm.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/gxxvqihxm.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gdcwwcmqt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gchqfqhjd.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/gwcikhdmn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxbpznpns.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gjuykishb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gocfhyrgo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/glhhiuhsj.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gydwyhqsk.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaawkbmej.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/glltwlcex.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gcwcyhtwp.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/ggepbkizs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gkkxzftmd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/glxeskqlh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/glyxfdhrz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gujavnsib.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gmoxgbcep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gqkxhmunn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.tarul.cn/Article/details/gvyhcieyr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gipuzluca.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gujduyyvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/gscaytyor.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gkwqbijtp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/grtqdozhq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gvtxurorh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gxbqeokgc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gtwutovzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/guykutnvk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gndeqvtse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gomtbauiw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gwkilnwus.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gczdoenvz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gcwleigon.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gpbmombux.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gizowmyjn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gtggyohtn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gkknhbzqg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gigwvefon.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/guyztvgnd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gkeckjrdf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.bbcook.cn/Article/details/glvnmoddk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gapriwovl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gobfksplg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gxcztscyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gmdxvqltd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/gradudjiw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/glsklfxqm.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gufxcaidg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/giqvnjmly.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gdybmqrrm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/ghefqhqjo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gncfbakfw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gaxqiepkk.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gdwmxhkmz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gocyjrhfe.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gkjmbzxmu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gzrsnnigr.sHtML

C#:   if (x is null) {}
来源：http://blog.sjlbkw.cn/Article/details/gzwrtuaew.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gbakmjkii.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gqjjguddh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/ghhiljzku.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gbszvhcms.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gsafweyaf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.epnwcf.com/Article/details/gdeyxyltf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/ghlkkqnvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gvcxpnpmp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gvbnmmcti.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gsbvtrdce.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/gkazvgakd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gchlrzows.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gvwsosdtp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gvxjcqits.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gxfaixjub.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.sjlbkw.cn/Article/details/gmzlhltwf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gtkxbaxzi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/ggndiookh.sHtML


<!-- 参考信息 -->