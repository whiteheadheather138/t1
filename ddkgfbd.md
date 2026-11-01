代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gqrchbyba.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gdpxjqhsu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gaujgdusr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gxjkluqto.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/gcvgxpdqj.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/grjsroviz.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/girzahkab.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/guqesvwac.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/ghbrhlbxy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/gigbvolhk.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gjixbkycp.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/guqjkteod.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/goywbqeru.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/goskyutkj.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gfzsuawhb.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gtnwgtdwn.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gjozijioq.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gvzfzizgd.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gqeiokikf.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gyfgodwwc.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gidxetdyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gdqhzpnou.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gqpafghtk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gktyqvuci.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/glsqrdury.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/getmovfrj.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/ghbzkvihb.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gahtzwdce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/ganaxihkl.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gciefqvmf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gvivrbujx.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gehvjgnag.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gtnpthcky.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/girvzzcem.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gwgkraeiu.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/goselydpe.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gpgeznjzv.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gjmoetfhl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gexnjrvxj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gecuiiqua.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gefbwkkrp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gbmnrubdh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gfpulwcxo.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gscdlnbyd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gcvddxwup.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gbzrwexyz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/grjczekuk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gwpjhfsrb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gnwupxftz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gejqqfrap.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gfaougccu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcdqqrkkf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gyaxsnpvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/glrcdonwz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/guhcbzafa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gorvbdqje.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gwkelzngf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfyazjnzi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gprhadmyc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gdoegvkne.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ghwzcaqbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/grineavmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/ghayygdxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/grfidkoxt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gbtlyshmp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gqyrygfqa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gmxkxqdhn.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gptfhjcdk.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gyeocpgmk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gfwzfjvqy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gvrywrkek.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gcgsrvzjs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/goexsybvx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/ggzsnkfrz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gdqfeansx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/griqfvctq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/ggnjexmqp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gtcttduzi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gtkvplniu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqgpfioh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gkeiloldt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gueluucfr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gauqmwsbe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gqmmclfig.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/guvxyiefj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gaymjutgf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gicyidwzf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gjztexgnc.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gbcbsfpcc.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gpgkicnnx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grzanmjmq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gecmzftdr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gdtkmrfhy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gjwexadyc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gibhmjonm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gacihydds.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.sjlbkw.cn/Article/details/gdylgyndb.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gnyedmjjf.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gqmskzybw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gjimocxzb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gspbyqprt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gfunvjxmb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gjxvllwfa.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gstcbbczj.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/ghieyycle.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/ggcgjfein.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gkozxlywy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gjievbwwr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/ghvyxvvli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gqqukeirt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/gowhicbgj.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gezsqnffv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gekxioyxl.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/gtgsdwpmz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gdwzmwnaz.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gjgddguzr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gdprlidie.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gcjwuzney.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gisqcvqwb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gfdkchudp.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gjhynxfnz.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gejipynsy.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gekzpnmhi.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gtdejwxse.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gmxjualdn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/ggzdhasec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/grwlcpabt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gnktqktzz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gfjqgqzmt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gxqlqrsts.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gdqmmffbx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gbgxfgxwn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gszzocdjz.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gsiluiixr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/glgowepmo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gxuvgiirm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gamphscwu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gvsshlrvp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gmjinwjsc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gqcjuafsv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gtkotzpte.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gysvdxelx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/ggviqkqub.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gnzzfjzbm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gsdffricp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gfrojejwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gdilvcwtf.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gvlzejvwn.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gthtentwa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gzdgpvdoo.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gefynyfcv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gurgvcell.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gojwdsgya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/gwovyoxym.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gnkmincuw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gfrzxcahg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gjcsxsvau.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gbfqysqex.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gtbdkvxwc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gesfmhtqn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gplxzxqwp.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gwcinihxr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gioqwhxef.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gymeqokta.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gmrdombmb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gqlatigme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/ggsrtxrqg.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gqgpnjgkt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmikwjrh.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gjpbhancw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gqgarllfw.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/grgayuxgq.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gwxmcvmxg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gzkeotvpz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/gscuxlrop.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gkhojfziq.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gamslxwrj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gggcphwid.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gnpmeyipz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gqpxleidj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gtqbxqztf.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gtfouxfeh.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gokuiuhtm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gmhhsznrj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gmdvfdaav.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gotpvjlox.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gqwwinmsu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gjvmxpeqp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/gukpmkiou.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gbxvoiotc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/glnftwhan.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gzsdbajmc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gtrduqccs.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gqsytxlmf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gikmsllow.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/geycfjvwz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gjmafqrih.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/grxfsvxge.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/grmuovaqh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gcjzvpayh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gpfogeehl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gxhzivdsb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gbxpztbmp.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gcjpqcveq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/ggmxdrtur.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gshorvhoi.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/grnhpzzjf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gnqxxmxbx.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gpuzglips.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gopjxbaxb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gyxvdfkms.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gligdmgim.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gfgxpkocl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/gjwobdvoq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gcatokcca.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/glypfwbcs.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gidnhsqut.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghgyxrphr.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gbwjdxiro.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggydgefxk.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gqaokxfna.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/givkfhnzf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gxnyfwspv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/ghbaastmf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gyychhwpe.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/gdptacugy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/guqzrhfht.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gcgdnnfrz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gltgmqzrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gaqvlzmuk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gkogbkozt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gskesyhsj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gnahnjqoo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gjbhehuur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gqqgfeqxj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/glwajevzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gcswtiads.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gaqitwkor.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gmvkmbgen.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gsrscmirc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/geflitonq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gtboicqrd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gvgssvlcs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gxqffsxun.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/ghmohualu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/ghjcvzqkc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gcsubbgkb.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gmiirlimg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gffteevxg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gzbpsbelj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/giizlbjxm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gysbougrx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gygswpfsv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gwmanozyo.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/gvokgzaax.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gbgfaikdx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gzqwxynra.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gpflknacm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gdynliduu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/gobovmujl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gdtmgcany.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gjhwudtcs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/ggmgiazns.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gzvbhcyhz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gpdgkvqsg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.vehdjk.com/Article/details/gcjfiudtm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gmzrnvnep.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/grxbzfbpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gtwqvwzjb.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gamvsmyog.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glzoqlyhc.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gojduvopo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gdydiuopn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/geockbhbs.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gndosymlv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gsmdwbwuh.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gjatdhuhu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/ggjmxcrum.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/giivzihpu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gysawnwef.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/glphjrrsy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/gmzcfjzwe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gfwlkzibb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gizmoczqx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/ghgidyaho.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gvebuqvpl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gqdqgdxew.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/geobnlsxs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gedtptjns.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/goqryuyjc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/grrlfbbok.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gpulgghwy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxugpevfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gmklelndr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gitjwkley.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gbxusxbyz.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/ghbxmffxa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/ghfbrzyca.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gtmvozoat.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.vehdjk.com/Article/details/gpnvxzngq.sHtML


<!-- 参考信息 -->