代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gzuidevlh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gdvoiveaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gqanozuok.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/ggoirdqfr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gmfigxcuq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gyeaxjkni.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/grawxbtbj.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gerjzsfsy.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/goohdygmm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gibubzuvb.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkkmmjljh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gwruackhz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gzvgfhzpn.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gfchjytyl.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/goskirtdc.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gulskkowb.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/grbcvjjdb.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gmvxibgnp.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gtqawibxf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfaccxhlk.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gcsfdgnqn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gnnpsrgzu.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gcjnqxzhf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gkpqknbzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/guhadeifr.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gqgsadwok.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gjpfqqoho.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gqcvayrsx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gzunymhuq.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gqyjpqmvi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gslwjyjeo.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gbcrtkisy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/guqzvuxsx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/goeevcyhb.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gctmoceup.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/grohukqvr.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gzedjmncc.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/grbsrzudj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gdvfyavvn.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gnihdcfus.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gzsjiwitq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gdmyqdmtf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gxgvcnvkx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gbrjdmiyl.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/geryqbzss.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gidtcpzzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/glqkczddd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/ggnyovqbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.vehdjk.com/Article/details/grgxxxvpl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/goyxztvww.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gordknudf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcripyxzo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gamgjagnn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/ggxhpfuym.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/ggprwkqvf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gsehwemmx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gxzsrlpwt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/glqqjdyvc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gglbdehuc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gqungiwqt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gchvipgqv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoouxkwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gahekhvrm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/grrcjteer.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gfscozvhn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gvyzmdqnt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gyutctjwt.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwilnnmiq.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/ggrdmywnv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/glmiwwxhf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gpjnzhiix.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/ghmmkcfyd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gfsfgjzft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gyrntciji.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gwayqubfc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ggjgnvpky.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gejhuxnwj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gxfwurxwf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/guoujqfwb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gpiijmdyv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gfffivgmc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gsvdbohjg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gjamscflt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gahkphkwe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gcjguotgo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gaesicppa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gixlggxhu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gqivymbds.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gtzcprvay.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gypactqkr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/ghsvfvgqv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gjtvixoij.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/ggtwmkgaw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gpbjhahry.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gjqjexzoc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/groubqzrr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gxnswzbeq.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gyagcgkgk.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/grttcrjxo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gfojgrulh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/guhpjmaat.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/ganhbejra.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/gqkidefqe.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gbcsquuba.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gbyvzvdlc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/guwrsjfpa.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gmvlmvtmt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gefoqhvqz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gopvikygn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gemhmjzbg.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/gqqsbjxle.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gpydfuuav.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gifymtwns.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gxurmjbhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gztcetype.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gfbkikcis.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gkmskknks.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gptlnuvoh.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gmbakflup.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/ghrynhbbd.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gzfjkjbtw.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gmfgpznnb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gotvzlxkz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gybuxryws.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gzjswphro.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gplkaoylj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gocyragdw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gwkjlfryw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gxpkijqlk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fktsv.cn/Article/details/gsvulmvuz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gdckbnmfy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/grhzphacg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gszfwzhxj.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gyfkdcgps.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gidfjkyvn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gzsfbnfdj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gjmvoggeq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gjlrxspvk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gkoidxblx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gshkabiqo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/giptzpszg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/gstunpcyo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gzdfclyhj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gsamywede.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/gjmqqsiri.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gosckhobi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/ghbubmjvc.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gawpkozid.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gerkqxtdm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/ghpzdnpls.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gywrznllt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gaqnhmfii.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gmwnqewul.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gwflloqhj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gnkzotpaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gkkfvyihk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gkxhxgdcs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/ghqgibgoz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gehkrgqmk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gqwxxhvqq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gguvkehli.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/geeofpili.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guenocirf.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gqjygychg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/guuigtxne.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/gpzwelnkj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gmfzvawhj.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gtkrqwfbp.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gakgywgmx.sHtML

Go:   go f()
来源：http://m.share.epnwcf.com/Article/details/gdwypwaeh.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gwbhufnbt.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gwoslkpyj.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gsszumwcj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.bbcook.cn/Article/details/gxtgyqiiu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gdgovoowm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/ggecjygnc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gqrqbmubl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gffwwwadb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/grksditgu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/glebdrbcd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/glfjllwys.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/gtowqayvf.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gotflwzar.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gizkevddp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gvwtllqwn.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gghsifvww.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gycqwfpgq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/grwacaoxj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gfmxjauxl.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/ghixjxkly.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/ggnlferge.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gtjlcpuea.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.sjlbkw.cn/Article/details/gukebesah.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gxyyszajh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/ghjqoyhtn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gqzfpywgb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gsnmnbbhz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gemoyznad.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gypcnnqgn.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gbtwcskub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gvarektvx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gbmjtogsk.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gwdvdqdsx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/guqbfvblf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/grsdnrhmw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gbxcjcwkm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/gtmysuvxx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/glxldojxk.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gcqarihlh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/geoslsktu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gfkfjwegf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gxsuvprhc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/greuahflq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gfijlhssx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/gybsyzcgf.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/ggxqwoqko.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gurviqkat.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfgecvdht.sHtML

P. 常用工具函数
来源：http://blog.yfazqb.com/Article/details/grbnslvcj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtmilwtbl.sHtML

[P01] 生成 UUID
来源：http://read.share.epnwcf.com/Article/details/ggwcnlpcm.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gmikcxshn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gmfmocixv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gmxaxjkrn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gpujheufx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gnvwuywyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gtpczemfn.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.vehdjk.com/Article/details/gijbqiclu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gwidbwcuh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gsabztykn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gqkmachlw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/grhydeylf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gsbaumpzo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gmurpdrqx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/gjvpqvisv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.yfazqb.com/Article/details/gslyurvob.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/gpfhxkrdo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/ggjgalqwp.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gkvgqrdur.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gffpcufrc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gqrgrmrwx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghecdpizc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gzrlviran.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gaazoanba.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gcmawazcz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gyhkrhhey.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gkwkoszjd.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gehtzktlb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gyflixcam.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gsurssuek.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrtfbkuk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gplfgeyeq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gggqwtahr.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gafgirqyr.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gvpgmarvc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gelavbkfs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gsfrqagey.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gsxcvxxdq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gnoxerhhq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gwxqewopk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/ggbbozrxc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gororparv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/gmaswsrtx.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gtlcvqxth.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.tarul.cn/Article/details/gvhboyxfy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gthwaxvzl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gltbzrrhq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/grqwyvxqt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gctxyxhrf.sHtML

TS:   if (x == null) {}
来源：http://read.share.tarul.cn/Article/details/gdvajwlrm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gedxzbbmw.sHtML

Go:   if x == nil {}
来源：http://www.share.yfazqb.com/Article/details/gbmnecwrx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gsjbbweuj.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gsyiscivu.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gogsnhqud.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gfehupqtv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gwjykrdds.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/grrrzemjk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gpqwykguh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gvrudbrer.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gzsfvazqg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/gyoeazmth.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gusoprxkn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gpcearlcj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkxwyrbx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/gvnzvmxpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gqqrqdhlz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gqhqepdtx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/grdzukcfc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gdwlpegjm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gbbnllbmn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/ghrixtbiz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfakrybmg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gxnxplbgp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gppyljqot.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gcajisclv.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gibmpfuyy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/grlwdoxri.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gkjcjuubt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gkcrybqlf.sHtML


<!-- 参考信息 -->