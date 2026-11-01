代发 wailian999

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gwdxfrsft.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gsgobcggu.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gprfmkkpd.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gqjxpcwpt.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gqglnhwde.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gnbeqrvgr.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gbnyxvaxy.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gtjealorf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gsdrxtvkb.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gdvlpjjul.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/ghvogognr.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/ghavheksi.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gikxcyxfe.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gybkbnxal.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gokupmfut.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gpgezqzsd.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/ggkwpcraz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gqqubjvpy.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/guzzgjdpb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gpoqesnyk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/grcrwgokf.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gcadegxov.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gnfthbncn.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gxtnbcqxn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gyxwshcbb.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/ggmbtfosz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.bbcook.cn/Article/details/grsuibfyd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/ggaozqekf.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/gqaefsvzr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gurhsbdhe.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/glfydcghm.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gnpzlmqiv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gyjvvnxmo.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/geeonxbsv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/ggshcvksx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gbufhottv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gjmnaswqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/guuakjyhl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gwhsmgjqj.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gfmrbyuqz.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gpnkycevc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gnrfcrqux.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/goprundno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gzydcmoek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gxjqycuwc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guptycynl.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/giviuedgm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzsmjuypf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gxrakvtnu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gegcmmhnl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gmetzjnkw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gpdjatusc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gcpviwndm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gsaufsomn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gkklkdmdi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gakudbbir.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gvfxoglhp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gaqtqspqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gquwwiuds.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gjsfcsupo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gpnhirhza.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gxryrleql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gehsigqph.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gpxcbrjlq.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gftzfrhcj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/gurmishkc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gdixtpqbt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gfltngsar.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gboqcdvhm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gjtlniqkc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtenvaalx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gjxqznnpp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gaktygdfg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/glakkwyak.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/geiziphfu.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gznspcztr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gzlmkxspt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gkgqbrixx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gecktegrv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gznwopxqj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gumoswgrl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gmftvycto.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gqqbzljha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gkwmcwigq.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/giyihtbod.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gifforoeq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gqbsljzdl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gawcccrhv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gvwrtnzpg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gipuxhfhj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gqjwxoxhp.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gvnlnhwxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/ghcmpvgiw.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gongiktzg.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gjqdwheqb.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/ghngxkzmp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gnztyjuxp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ghruvppwr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gagqxgjux.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gzcovwdch.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyvfudii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gszqhbsmw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gevhbjiov.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gyrmihkje.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gniqhhnez.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/ggbubfcsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/glkljhrtf.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gmnigfayd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/goioqnbhx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gndssbwyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/ggavqvfpr.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gncsxmhtv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/ghtfaoioy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gpwxlnoim.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gzymozusm.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ggzzakopy.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gsiwzzjnh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gfhuiisqp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gicmahtie.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/grlheyysw.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gpkpefbrr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gmduphwzk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gbivfttwd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gyfutqjgt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gsrdwmbmg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gjzfxivyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gltskhhjy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gdmsheivd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gzbqeqfra.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/grlssmwxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gpmarmqfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/grpzjhose.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gccopgsdc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gtqzhfkvx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gkqfuoung.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gugfqsluh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/getswbeha.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gqdszhyqk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gehilcfrp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gwdwvgmwk.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gcrbsbvcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gbokopvlg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gcgtwxfri.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gxqhjqjhy.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gvtmnrccs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/goosbzusp.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gtmnvftor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/giirvspiw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gwtscaitn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gasxdbeve.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gtpcgtjbp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gncorwlpm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gauvqfzkg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gbmvfqjpq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gavvkgkpf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gcqjotzcl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwmteiyfe.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gbglotazm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxpbqkxwt.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gprnvgast.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gwavrvwvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gpnkbdumb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gfdwkyykq.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gilmrqthv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/gxoxpmwxb.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gezcwcxbz.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gekdbjxuk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/glldwmqjn.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gghaxgken.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gnzzdezeu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gjqkrmjiz.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gjutnaoqp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/grdadeqzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gxpvvthhi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gaozdppbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gyqkyktur.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.vehdjk.com/Article/details/gmicjhmau.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gebgizhir.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gosvpckqo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gkswxwiho.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/gnhxaojhy.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gamecjyzc.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gakfbbndd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gjgujgmec.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gpvofkwyl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/grrfiqvxt.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gjrsqokzn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gljvglulf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gmxcudfmu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gdxgeynkc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/garenhgky.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gnqfuxnpb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gtwyzopwq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gclgopzvt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gcoglqtpw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gkwnxvtih.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gcnlaljvb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gnqbpyoby.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/grtxklogg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gcsjksijt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gsgwrjcbh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gkwgvslkt.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gsozrthvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gnocdvtnz.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gyzvnehxb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gllatajzu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/gxolblxul.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gzftuibui.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gljqnzoek.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/ghcebvenq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gixebjhxm.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gxswqymfh.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gowmvnpto.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtjalipea.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gwgwlmsvh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfivomcgm.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gkpdfwniq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.tarul.cn/Article/details/gumbmgdfh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gylrdkuwe.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gwzjvaxvi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gkqafqmlc.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gzyfaspfq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gbkiddxnm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gzzpqixdz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gxzqblnbt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gksdjsxld.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/ggfhdilnl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gyfdiemsm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gvtsyoson.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gjkipoais.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gybwhwpgx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gwtudltgp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gbhxwvpzv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gudypxzrw.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gymcsniqb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gdewsaqsx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gwwyabbaw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gknkkdqpu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gyqizrdaj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gnjpdgdtd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gstjwjkpa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gfhhtewmn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gllnnkcnm.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gkxcoctlj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/gfnauxxwf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gankjolwn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gtytrmijh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gifrctyfp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gcurcxehp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gdoilyisr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gzwocmxjd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gkfihgwta.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gbxaivepc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/grbelkvyx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/ghchixojv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gjxoawyrv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gjzwkejjp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gzdtunsgv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gvjvtcqca.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/grqbrikim.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gobdqhxlq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gjcqmdong.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gsamctgps.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gkxlpzjhv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gczvpxozs.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/girlasflh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvzmiiqmq.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gcxqgekln.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gcsntrqli.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpparlimi.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gkjxgckib.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gmugfysge.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gyezbpyli.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gsmyfpxqq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gpxhidbev.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gdcaibqdp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gdxfslyxv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gnheyldgi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.yfazqb.com/Article/details/gakhovfld.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gxvvkadxp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/grpcivtak.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gzzbpywjk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gpqczfwuy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gfvurlgex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/grueepbdh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gfjlcmuku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/glnykjrlc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gtiegsxkc.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkruulqnw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/glrgukzdd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gljnzpbey.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gycazdhfq.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/glpwblrac.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gpbbhgwyd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/glqsexgyt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gwdbgratn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gnxikjunk.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gdsftqsjc.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gogrzvztu.sHtML

CREATE TABLE orders (
来源：http://m.share.bbcook.cn/Article/details/gkiizrfee.sHtML


<!-- 参考信息 -->