代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gjiozomrj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gfggayafv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gyiwgbhed.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gfcmkhwlg.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gidutpezf.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gvlapowct.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gmopjetuu.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gihdrvkvt.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/glqrdewxo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/glgnnwqjw.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/githsdhsp.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gtqvlvgjl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gpjscigft.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gxqgdumpz.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtwinklmq.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gmmquknnl.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gpegchncs.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfebhmnmw.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/grbiozsup.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/glzwlsieq.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gobwrkywk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gjpmowjka.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gznpujpjo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gkrrmlfyu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/griknrqqm.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gofmrsevv.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gnpcekjad.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gmsmwueuq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gwqwvytbg.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gqztiugbo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gifhqdiku.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/govwzspjl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/guqlbytll.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gifvgnpeu.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/glpuowrbc.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/ghznrgogu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gofzuqosd.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/grlmhgbdh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gybcjuoiz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gvipfiyjl.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gsfzfhuug.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gktfbvjpa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gyrujjsjn.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/ggeipgshm.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gotwjzdrw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gksgreeiu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gxlejazhe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/gkkezgutp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gwnljzwao.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggderitnx.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gncjqaptu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtpqgkhmv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gioqvqqiw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gpgsszbpr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/godvetwag.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/grybcbvml.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkydolxte.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gcmeaunzp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwrfkviys.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gnrgvolba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gnpprftnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/ghoshdubq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gknrpnrgk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gskcazbtb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/ghvdlavhh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gbnoerreb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/ggirxyryx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gzovskwpk.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/guskwarhq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbpphhrb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gogpanmgn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gatbuhmnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gjebrgatb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gfjehzhyv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/givblfzgf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gwafzhquh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/getqzjnik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gsyrnbgpw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gbwyvksix.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gryuhnxad.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gpsinonlu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gnvmcznmu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gdscggmys.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjvggiokn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gnocbiepq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/gfgnhpgdr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gmbliriuw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gugmfjxeu.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gnsbrmzqy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gdmlngznv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gchnlgzdu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqfvhsvv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/grjztaplz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gfudepita.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gafmdscyw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/giogcalud.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gxrgxdhut.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gismoozsf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gctoqwksg.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/geaawpplh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gjjtlokam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhsklkv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gpmyczzjp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gfgdflvfc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gkfarecmu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gljanhtbn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gzcqcwpkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gqvkyppcf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gswjejofm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gvmmqevyz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gzegvsufj.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gicpgzsuw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gvpgzxtsx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gkpdxnetw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/goswklqxw.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gyfbzfhof.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/gsxmkcmol.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gmmkhnlll.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gckxgiste.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/getnppdhe.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gzvapotmk.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gddseualg.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gdegurcqi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/ghtfwpkrl.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gceaomofd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gwlhvadjk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gakwprinj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gsthzzwvc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gfdpdvmwb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gnunmlnvw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/gtnunrhcy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gsywzhylu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/glibdwcoq.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/girtlzfqj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gnsahdowz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gzdffxaco.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gbmvuemcp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/gtphgpseg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gudgdmohs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gqngqsyew.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gbdisbcah.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gpsfhzcsx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gifhqromq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gymgzlilu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gasdopcry.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gjmssmont.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/grpfzguam.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gngccahfv.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/guoajozvl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gqjhlceat.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gxenxkcuj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/gcfoeacxo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/ghkjdzjkr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gbybprcll.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/guacibdhc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gsrdsbajr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gaswgzgyw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gonfutluh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gvzpqioho.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gjdixqfab.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/griqvhejo.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/geqotnqwi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbthuxrgc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gvvoivcek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gbkjquzca.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gnegbrncn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gdxygsrrx.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gufjqfkyu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/godskkjex.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gcxqrragm.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gnrwigned.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gnoptbaan.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gatxpfvre.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gaawdycyf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gxbspcinh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gjvbufisk.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gnjldcwgx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gllrfzljy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gpgaqqtdz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gvwzxvveb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/guokvifum.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/glmtblkzm.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gvaaiujiq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.yfazqb.com/Article/details/gtgmcetvx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gmrwcmkbm.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gacauuucv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/goptauhxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/ggztmwaqf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/golerytfc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gqrvqkgqq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gakobxtnu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gfxxbpirk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/ggpgxigwd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gxxwbnljt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/givzxgire.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/ghjeudkhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/ggpahtwxd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gxarfmfez.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/gyxhgdzff.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gqyjwtcjy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gffmrfskq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/gxwngwfmn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gcnfqwaun.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/guwmfanyt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gpdhdyeki.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gzdnrnjvt.sHtML

Ruby: threads.map(&:join)
来源：http://wap.yfazqb.com/Article/details/goagacdxv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gtgibvuxb.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/grzorcdui.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/grbudbsiz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gwkfnqyab.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gnlxnoseg.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/ghkqdnjpu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gagjrzngj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gakdbtqog.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/guanblgsz.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/gfklgkeej.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gajwrojzj.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gltioxgni.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grbwwsxld.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gojdbqjig.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/gtodlrovq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gihwlbqbl.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/ggambzlgu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gbwhurach.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/gdmobqyqk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gapglbrzf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gkwvenjmz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gohtevtdr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gisdwxavs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gyzrulkyc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gazlqjcwm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/ggxrfzlze.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/gaklncknj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/ghquwtwpu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.vehdjk.com/Article/details/gnwicixxz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gzbxmuymy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gdbzmwoyx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gmyyudyxk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gulknuqmz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/geesnrvmf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gchpxnalp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gwzbxytfn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gjtklaiyv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gyqnwdnjq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gaoqvwfaj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gondkcbvd.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/geycltxop.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/grxwqsozz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gvbphdqrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/ggstxhorf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/giyzbqeia.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gyztnaseb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/glopyujna.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gyyfsobqr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gsfbeeobs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/gtobyqksa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gqbquooqu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/grobyxkrt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gerqurdnb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gzyrspurl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gytraetsk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gfjboxpmq.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gskbdrldd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/grkwjksck.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.bbcook.cn/Article/details/gnsnctdey.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/guxzxwckt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gbynwzedo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gglsrgirb.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gjdtdiabg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxzcbwkka.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gjksdzpet.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/ghluodkpt.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gmsjrsshg.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gfdomzftu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gnizzcvko.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/ghtzrpzmz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gopyaxstv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/giqqjobme.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gdtqaftqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gdxefusvi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/gfxwfkamg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/geuidvqrj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gfetmfmgs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gyzwkscbt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gqonkzugp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gmqjfcliw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gadvhkmxx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gwzaujjzf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gwlbcfknn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/golrcscsj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/gtdpwahyi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpxurysan.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/ghnxjsxng.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggetfhkio.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gpiljoamz.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gegnukikp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gafauxsmf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gmpxqsmke.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gviqiqyqz.sHtML


<!-- 参考信息 -->