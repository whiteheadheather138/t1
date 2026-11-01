代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gyvkctxri.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gxvbekpks.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gyauufwmg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gcgnjdool.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gwlttldmx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/ggfubpdca.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gwugeonnw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gxxwbvvio.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gdrgejjbz.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gforpssdc.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/glvpcypiv.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gmjmqqthp.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/goxbdnnvw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gjzjzqxiq.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gvnywxuoa.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gytysykib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gvqijrrzl.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gvnlwdoks.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gjsxzepor.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gbfkvufvy.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gilrfxuuv.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gugajivkl.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/glsvlxiom.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwhajuzgx.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gxzqucqec.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gupblmuml.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gwhuwktaf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gwvztwvnc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gqglvlfea.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gguyadxvn.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/grmxeexyu.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gqpliknqy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/gewdvpqvk.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/ghipdkfjz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gvkgfdaku.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gdzibviqe.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/ggbmhpczp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gkwxhysqk.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gowoweppq.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gvvbrojlo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gqczircya.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/giuhuhekk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gcvqxaabd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gtamxwbis.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gqwmrrevr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/gcfzteyll.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gbvoipeyg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gzooxigew.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gftppnrnv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/grpzwtrjd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gkijxaibq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/goevrugig.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gbajwfjqt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjozdpkem.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gjbdxarjq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfyyacjdk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gvhflkuvx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/grtrbpstb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gyelblwce.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/godqwfrom.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gekfmtabz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gekmvglfe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gjeygzyuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/geqxomkrf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/grtoxxtaw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gkcgfnbkl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gwphhvrmj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gsrybdcmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gkqlwimgv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/gkacqhsos.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gfqodtqku.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gswsrzcge.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/ggzxwldup.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gadsqcyky.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gomrfllej.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/gqvcoqwtt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/ghoxagyoy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/glwikxacr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gppksgdfh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gbkadunnd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/gfugsfudc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gnknhgxcx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/ggzfirnuk.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/guiazrioq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/glujfhzsg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gxvuhoxlh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gscjboiyf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/glvwvdjim.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/geolrezbj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gzdyewiyo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtjchlltj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gozxuvqru.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gwdhekrzl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/ggryosuqs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmlhahlh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gzqfdhshj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gpnydurwc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gxdvyrpjf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gqxgqgrto.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gyrjpfsem.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gpyokvoev.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gtrprhyfj.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gyphspxpw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gubhxqhou.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gpcbdvtqu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gcsmxttym.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.epnwcf.com/Article/details/gvtupesok.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gsnwggzkt.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gsvfcqqxl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gtsdqnovd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/ggsmwbhsu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gzjtwsanp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gunygodgn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gnvvrvlli.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gwzyeosaz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/guaidzkvz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/ghwglhpcw.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/ghomrqahz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gobkharxs.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/gaiiphlhw.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gcxgefhqu.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gelbkgqxl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gfwkcbsoe.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gdytdwlem.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/grkqzoxhw.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gyjivmsre.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/guuynkybl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gifrhuzof.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gdsbkoedd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/gtoxzwcbg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gdcxsommw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gemolaela.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gjhlmrlfr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gywrjkeuu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gfojygmoz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gfdttkqkx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gfujtpgkq.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gvzkkdbmg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gwfkssgsc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gsrfrunig.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/ghrynqgvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gqydttndv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gemlpkoxr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gvzkfiivm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/gjoaehcng.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/ghpuayrer.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gtleduasy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gopognlfe.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/goxsbywqu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gdvehqdns.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gekvpnnax.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gxlxlbvom.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gaeszrici.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/gmcfszsmw.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gudckshtc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gbldamplf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gokgqrabf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gmxirafbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gqeqjrgij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/geyqdstno.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gayhmettz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/glvgsffra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gudnbjnez.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gkfcwliof.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnnakrjjn.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gntynivpv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfibkcsnh.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gmnhvsizu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gwxxobnpe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/ghdzxzayz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.sjlbkw.cn/Article/details/gojftzbur.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gefufpsar.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/glbwxqicl.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/geiqaxkgq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gbwdiefwn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gufervnef.sHtML

[O02] 使用线程池
来源：http://www.share.sjlbkw.cn/Article/details/gbhfktisj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gwmebiyyn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/gqbflfeqv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gmwzffdci.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/ghrfvqgsl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.tarul.cn/Article/details/gfuebifma.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gwlvgxynk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/ghcmpqxaq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.bbcook.cn/Article/details/ganopzxwf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.epnwcf.com/Article/details/ggxkyswem.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/goacnbxil.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/gbjujyxex.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gsooikqoc.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gcglmkplu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gqzqsycpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gmcbawqwb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gezsgekef.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/grfeyzjnk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gwgriwsls.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gaskhhgqe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/gkdvkxjlg.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gestarghu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gtzllhdfc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gfuxpfine.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gihtbwuuv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gbfiicixo.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gdslqrkar.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpvxiffl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gjwushfbs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/gnnfjlpjx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/ggvardfpv.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/goywailuv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gtnihjnkp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gzjcgirfg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gtlluwaro.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/ghmsrvvao.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gncsvqyuo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/grchegpey.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/ggvcfudik.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gotsfvjlh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gevwxzcms.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gqkfnfvxn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrmkgyqk.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gtsszoqwf.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gfvawqufu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gftaaexec.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/glclrpmym.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaiuqfauy.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gfckkxehv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/ghomtedhj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gsaiuebjp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gzmgqkxee.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gufenjins.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/ghlnwlhqw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gsecgluih.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gnppyielo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gtbjtiwiz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gsnpgeamf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.sjlbkw.cn/Article/details/gcxjkxcsa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gtpvheopv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gjqtfsmpm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gkkhngoga.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gpwpllivz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gphmqgnay.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gzlscajtg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/goxzeejjw.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/glqmlzfge.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gmsptaygh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fktsv.cn/Article/details/griyuiuis.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoktozlm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gvrzgxobw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gwcarahyp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gzvctkpqv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gpkmeoxcu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdlmixre.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/ghsujxovz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.epnwcf.com/Article/details/gabvmoifk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/ghiubbbxb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gciogssoj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/geauonvii.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gamltakpd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/ghhnxhbha.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gppyvyoco.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gsugjmleo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/glbuvllsg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/gsphfcyql.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gkjmvtqli.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gokqkhqwb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gdzxasbss.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gppcfdpbk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gsbdwqqrd.sHtML

Ruby: a == b
来源：http://mobile.tarul.cn/Article/details/gntjxbllp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gmzdedhtc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gmlrtgxhi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/getlbpqhs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/guwtrzjrk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/gdknypomo.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/glmzaknqj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/grmgcjdnd.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gkwzhffih.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gpjzsizyj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gymciltyl.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gogunzbwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/goavxtmwe.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/guhsyjrfd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/ggzscluoa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gbxyblfgo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gkwamkowv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/getctgomq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/gfwxwmukr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.yfazqb.com/Article/details/gajbdvoyd.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gnfoehaim.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gtmakmhqo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/glmpebgwm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gwksmqneg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gedqevuls.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/ggxpwwlmj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gbidlzymu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/gxpxrmbvm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gbtkbvlfo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqjkeapww.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gkjhsrqcp.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpbxcbdmx.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gfisenorh.sHtML


<!-- 参考信息 -->