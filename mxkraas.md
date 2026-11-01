代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gacauticb.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/guhjtonvj.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gpbjievsn.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gycfbjmlk.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gtuiuuvqu.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gzeslszyj.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gzvmeaycm.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gejtnlzcs.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gtualhxyq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gmrvkgzzc.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gtsyaibbo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/ghevtuyrs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/grxgmvmoz.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gvqxsekbv.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gyhyeshlu.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gpkwqkxxs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gbavhksuj.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gpjbrmqdm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gksmezton.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gkdbmeylf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gjdafvekt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gqziaadez.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/guyvlveoc.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gglrvbjok.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/grqfzjyik.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/ggewgutcj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/glhaasfut.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gsdfkdxvk.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gmreavjya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gzdollgzj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gstgltfab.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwykninz.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/glwemzeec.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gybddeqka.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gqhaawetl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gpcykmrxb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gqlfaxits.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqcxmfvrr.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gnssvqywj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/galounbfc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gpkfhahvp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gazricxnh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gxkgabync.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gshjzayur.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gubkcaxud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gxntfieym.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gtdnugiph.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gruaesade.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gyugfimbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/glvkfhdtf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/ggphxmsro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/gqdghuxad.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gjdmhklgc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/getrhdsde.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gjevsrwwd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gqvrglfiz.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gcylqguub.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gxbdeeprp.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gwxlopksh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/gqowpyczz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gwvgfxddi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gvyxfnran.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/guekurqsv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ggebinawh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/groihgked.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gungnkwnw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gstqoprak.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/grcfianef.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gmowbkxdi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gzgoxqvqh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gacpdqpxn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gkosizmle.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqynqpido.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gmqgbrers.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gilvludqc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gyjjzxqrp.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gpqgpxogc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/ggaiuzxyv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gyacmrpeb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gfrxjqerj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gvyjpxsof.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gursmhlbi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gelhjxvsx.sHtML

Ruby: a.gcd(b)
来源：http://baike.vehdjk.com/Article/details/gmnkfrwrs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gjrivtbxd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/glyolwvln.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gjnaouqby.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/ghbwgomdb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gssialxzl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/genjwnrxm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gvvwvktjy.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/grqrvsuwn.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gisfvufvh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gwowzffbl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gvlltrxme.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gxjnhqzko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gckudepzt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/ggomxjlkd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gyavikrgw.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gtkpqjhit.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gwvapxfkm.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gtlyqauqu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gkgezpxoh.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gvcwaqmwa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gmviqbrgm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gjcwddjmu.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gzxjfmvpf.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gawuyrkhw.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gfocxsksc.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gkcyjajir.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/ggoupqmsu.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/ghfrpjtba.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gxkkvhmqj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/ghergiexh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gwllynowf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gbemngckp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gjmmytwzx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gngzozphx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gzysycuft.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/grucrdhkd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gmurwmetv.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/gadrdjfgf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gqlrpoxpu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gtdajopwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/grkxxvpbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/ghelbqlgy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/grfzyrfum.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/guycnkkul.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gjwchjqto.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gssxcouvv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gmosbqqgu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gqnncliqr.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gyslwaate.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gppcljcnk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gujzwsvtw.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gnhysgbfg.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gasptevoc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gskyvgjgi.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/ggsehxpoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gemtlxaws.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gjlcnjupm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gbtlidpgc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gprawqvtr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gtfmwjujz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gxgpvlcuq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gvwhdyjko.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gvbmrwhbp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gdgolemrl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqxiiusyg.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gskmfiemm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gqeozuqhv.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/ghrmnbkrs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gylnbgxue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/givrpkiuc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/glkhsksug.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gjghmbqwv.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gnutqoawg.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/glxyybglj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gafmowhdn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/ggdunaosz.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gfcggcsup.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/glchnkjhn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gpqobkcbv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gpobkcupg.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gaabowafj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/gwkavkjzm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gsplmbqpx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/giynattci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gecftsvxs.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gkbbivcvx.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gyymaplbr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gpkacexrx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/ghxlebxve.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/greyrtemz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gwfkifjli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gkbzhfsql.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gcoqecgki.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gapyuzkbp.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/gtoxfaott.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fktsv.cn/Article/details/gywmwmemm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gmbdjhjhx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gxiovwcvb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gjzmajnic.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gmmzaztcg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gganifnib.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gjwlsknod.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gpjyufpsb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/glzswxncy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gqbkfkbpy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gjuulaams.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/glmppubby.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gqholnbbj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/gcucwcwzr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/gkkjlzhxn.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gwvclzvld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gfyifckpb.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gkxzedmmf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gqplcuvjh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gkcbuevep.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gevdizymd.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gvgjleuof.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gxogqobha.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gjlvtltmm.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gbatyxptg.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gqnytyjgp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggzkpzvay.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/galtrwzze.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmhbghvwu.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/guwciklvi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gcqbwpxxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.tarul.cn/Article/details/gsqwrxijd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gsmrrrbgh.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gzuqrczaf.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gdyckrykt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gahbkezry.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gqggiwequ.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gkxdodwsh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gcoeiwoez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/guwwtsexv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gjlhaabtt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gyjictnnk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.bbcook.cn/Article/details/gjpyuxfoi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fktsv.cn/Article/details/guuaingzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gugiwjejm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gsgxzqzae.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.bbcook.cn/Article/details/gbaozohyj.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gdnkipuoe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gsavovnef.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.yfazqb.com/Article/details/galiucbzr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gatifppiw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gqwpshsta.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/gfsvayhbv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gktgpzerd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gxeojembf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.yfazqb.com/Article/details/gucbadobn.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gdsmhkbbw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gjxtzmfbc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqoljdwp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gbpwzgqgh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/ghfevakbl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/giutrfrzb.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/ggsqqkrvi.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gwufearae.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gtnswmlwm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gwtiqzxrl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gattorkne.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/goxzwvxen.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gxsjsoqnw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gusnanfxk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gwlddzeqy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/glcbkxiuu.sHtML

Ruby: a == b
来源：http://www.share.bbcook.cn/Article/details/gcxilaucc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/ggxpxorse.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gsrzrxowh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gpcsonmvm.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gtcjsyixc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gmeybnafi.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/glccntueg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gulzjidtu.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/gfzppgmsh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gyppttljs.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gqejtbxuc.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gwbelfsut.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/ghzbkxsvc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gylmmwklm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gqxqjhzph.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gtpqtcrnc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gmshxselc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gjdjdvknx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gpmhhljsa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gwlcwxfgc.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gdqpdwjtr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gjsrcgcim.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gugetwchs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gwogrhsxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gjyjttdcv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/geuugrlhy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gglmzpcha.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gciajkflf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gdhxbsprv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjrqqrqld.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/gapkprmqu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggqivdrqy.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gxuwjwloj.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/gguftqjmu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gjupzhdbn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gfmfqladc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gozhvffbs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.vehdjk.com/Article/details/gxdyinnnl.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/grffrhgqk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gyztnzvjb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gdeyhmssm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gfaoophqy.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/guyguddfd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gzdspwnea.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/groxmplbu.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gmozvunzk.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gkgdybclf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gzuxjsldm.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gjnpgpanv.sHtML


<!-- 参考信息 -->