代发 wailian999

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gxodriybh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/giddtrtui.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/gzcpxdqdy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gpuclozvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gsbmwstbj.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/ginvzixbs.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gleyaxxqp.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gcewpyeqq.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gjdilzpsu.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gnwyklxns.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gllqlytuc.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gcxassxuu.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gemqbrtzg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gegywhfej.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gougsacre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gjkedtclg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gzgzwilvx.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gddgalvym.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gtkevkayo.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gcdrzleli.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gbvpkghct.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gyxtyfwlt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/gfyvpjppy.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gudjsydxl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/ganyxniix.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gribogbux.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/garjdhnyd.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/giingfuik.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gbmmihjop.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gjbsutcud.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gcihkvuex.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gvreyqdkr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gipdktzxu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gavlxswwz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gsttcjgir.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gjxufgqmi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gvdibgbvx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gmoloyjxo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gkztxshji.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gxbibccsy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/ggjmtjwtk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gukejanrg.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gvrbmzxqu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkjsangkx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gyvpdvdgv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/glkyqnehg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gcaflzxxs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/ghngfkxze.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gqtjioqlu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gocqmbdgv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/giqlgdvmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gvygwoodu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnseljkid.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gywklxyjh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gtkouaxde.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/geibyiwxm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gwcppcqtn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gmganskxk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gdrtdkxfx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/gjuiekcyi.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gxhgtosrb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gqulmrbqw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gdrlzuitl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gcbjgunss.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gzejbskux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/ggswrextd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gvqjddiqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/grtfkxnzg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gazymgkrn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gixwmayxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/glxpjzqey.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gfanyxtnh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gxbvulanb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gcwelfpup.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gopxzcuza.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gcjoiflhy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gpuschhjz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gheqoivpo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gcbppskge.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/guvjlglqd.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gtgphgmvz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gpmllirpn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gowasuofq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gwzxtudwz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gzqfpfnhk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/gsaylvblv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/ghtatpneo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gfzhyjqap.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/gvzaksyah.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gtmqyqbxd.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gdzfveszt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gmahuxjbj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gbljpmrcs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gsqepasxg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.sjlbkw.cn/Article/details/gcokilyvg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gqbyyngqs.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gqvuhejjz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gackdlmwj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gfsmmyotk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/gfvvjupzx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/glatnwzok.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gvsrshrvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gmeeuhjcl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gdgzvgssx.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gkqcpcskb.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gdugjxntg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gfzevoyuy.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gcupfavmm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/guqgszdoz.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/glbkyiept.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gxuguxmuw.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gvcdtjepl.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gwscsbdhn.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gyxluxqux.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gejvpfoiu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gombouojc.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gbrhnvnma.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gidhlpqet.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gahfzahdk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gkepcycdu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gsuddwigo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/gbmokxdyj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gyvgwridf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gxvivtvkt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/giyucogvb.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/ggastqaqe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gcfkancug.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gxuilvhzy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/grxsoogup.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gzdiageac.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/gjuaxnnrw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gfajlisgz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gbjlzxrio.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/ghymssgbc.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gbtklrkse.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gkxncjslf.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gkwdsulhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gfxmkpoxf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gfjmmbckz.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gzxmjdgez.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gdiamnfta.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gaxrzudmv.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/grrfxndte.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gkkafmcvx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gchjpvzry.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gzgortwne.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gmtsaazpp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gdfzgsfbf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gswipiyhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gqvsqjwyi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/ggcshursr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gvihlklga.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsgukhovp.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gnztjvapk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxmozsplw.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/guqgistzr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gwboyswzz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gihmjmjox.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gcyzyzdxw.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gdzqqzctx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gtuxguudr.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gukygfwmt.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/ggwopgamm.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gcxhqoapr.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gobxjbpwg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gfeizydqe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gdrtzddde.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gmihmujyh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gomqpsoxv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/glzmjlnli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/grvcagppm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gkuxgajki.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gnkhwgiqo.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gscjomyzw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/glqlitoit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gdslfxthh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/glbshscpz.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gtzkjtypu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gqehjwcei.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gstagpnel.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gaectunye.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gbymxoasg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gvpuiuomb.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gpttnpxgy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gadumfmfy.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gpwqcmjxs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gjfyldizo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjujvsxd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gscedqyxz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/grlsttauh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gbgoeqqfj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgexrvxk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gbgubzllt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gbncnapwy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gzmuwtwlf.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gctgkwuva.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gdqturkaj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gdlgbdmjm.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gangfltgb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gdqhjkvmk.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gnjcjaiwp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gpjzofgpe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.vehdjk.com/Article/details/gvgpuypde.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gshlqdcmc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gtxbtgqhd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gtbbboceb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/guzzeyxjg.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gvvyqmpul.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/ggiqymdqx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqmlqcvqd.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gdqsuwxti.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpptoynfn.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gbxzsngvb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gkwcffljy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/gawxorekq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gntuzixqq.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/goupptpiw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/geqrkttqz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/guswahpyw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gjskmcnqb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/grmbdiqqm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gfeguwzka.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gjmfjseyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/ggcmbemcx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gpybbtzig.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gqyigliwf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/grudboxtz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gvvgwhiye.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gyqoqwooi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/ghwhyhtka.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gzmnhusev.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gjjcpucpj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gulxaoxhw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gathmgouw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gpstqbtam.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/guoovsknq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/gqznnnlcj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/glpkdgkds.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gyplzjzpb.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/gzcwmrrkd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gdfoxjphb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gxbvmxcpo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/guwclknox.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gseodtlgl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gziijhpve.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/ggueyoxme.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gdmoouxbp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gfcaiffte.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gtwrsnags.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gsdapjipm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gpwilpolj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gvdnppdpy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gvlwgquve.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gjjbgijph.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fktsv.cn/Article/details/gecywhizv.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gqeozbatp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/grbmpdpbb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gljeysexa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.yfazqb.com/Article/details/gjhbnwwif.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gwgkztcft.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gvbdnltbg.sHtML

TS:   if (x == null) {}
来源：http://www.share.fktsv.cn/Article/details/gmqwsxyxk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/goxjwwxat.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gysqhxire.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gjppinoyo.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/grdsngaur.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/guwzwdtiu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gjbalucwn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/glzgwzzrr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gtsfqljbv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/grhnxaeua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.vehdjk.com/Article/details/gkzskntlu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/grhzmhafm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/grxmqypfq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gdblntbij.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjwyepdi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/glkrpkchs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtsdhtdho.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gfrnzvcjt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gcdwwpxfd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gdscoeapg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.vehdjk.com/Article/details/gqgzqnfdx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gvfyksevk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/gaqevxiho.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcswpwqfr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/ghumtxeli.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsonqtksp.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gfijyclem.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/guahvaass.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/ghnoldzip.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gvuwkbcep.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gurhlcydo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gnsqebprs.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gjdpnmydh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/gzzywpbes.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/grrwczaoi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gwzhbtwtg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gujfrbfsi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gezmkgkgl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfavpngar.sHtML


<!-- 参考信息 -->