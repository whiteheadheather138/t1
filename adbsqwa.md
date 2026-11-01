代发 wailian999

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gtirqmndg.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gezxpsrmq.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gzdfdvngg.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gqigybbpz.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/glxaqpxjc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/glzbdudsl.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gxnovtwje.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gikwyucmt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gqwelemxr.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/grfwoqmnl.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/gxkrksufa.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/girvhancn.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/grgmdunqi.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gydodtzxt.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gexzxjrtg.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gilidisko.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gftenkelo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gmwueotcn.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gnwclvsfq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gudnzzwlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gkjoxwpoe.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gkvyjmrax.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gyuefibdq.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gfwkyiozn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gqnrqhthi.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gkpaqelbo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/goswjfbaq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gmvcvgtsg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gmfiiwwdb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.yfazqb.com/Article/details/gejmltthj.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gsjxkighw.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/glozitywg.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gwtzchjvc.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/guszoukhd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gjxrfsrfu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gvlxdwlrt.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/giiyrqdtr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gfamapwpf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/goepgndix.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gvvkdkxna.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/glowboxib.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gbxbulibl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gpbvmpfxy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gakhvkwqk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gwdwsbmzb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkyzgkizg.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gxhwxrcem.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnczmyngu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/geoaonexz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gdwmmxyvt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gkjuqhwok.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gmdtulrjw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gqgpmsvfs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gvktlrjxy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gzjvnxchf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/grlschdxt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gjszxopur.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/ghoxojurg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gjyhjjdua.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gnicjhyis.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gpwhreodg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gfxorgoqt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gajmapzrz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gvwnxbegp.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gbvsfysqm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/gwjirwkjl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gbmxydmoi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gphwuinck.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gkatkanrk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gqlhathkk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwhqxwau.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gzbzowtwq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gtflnpqwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gxzetilzj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/glqcuxhmm.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/ginqtwvfh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gnlcvytqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gmsmislyt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmnyzco.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gdqzoqzep.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gilrjdxpq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gbkqfoftz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gfvdloslj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gxktuwtil.sHtML

[N05] 最大公约数
来源：http://3g.tarul.cn/Article/details/gohqvpkoz.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gbsuesrff.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gxirtommm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gmgiiwcdr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/ghnggjhcs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/guwrzdjuu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gfmdwwtsu.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gyyzcvnhk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gojjnnuhu.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/ggnvaoslu.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gddzuvzkb.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/govnfkpim.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gzauuvbkl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gyjsjoocs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gjwruzqcq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gfhqlxyrz.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gkeufbsic.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/geuvxgbrh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gpeftxjat.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gcykgjzkb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gvsqmhebx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gktnaswli.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gmatswfnn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/goucwbzrw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/ggwgtrueb.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gnrpdueed.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gfmybqeej.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gxmvwiiii.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gfhzokvur.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gngrqhlqh.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gsxfpwjrl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gurjitfcm.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/ggildtgot.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/grgfngxqw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gnrxoafks.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnofpqfmf.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gyirtwfuk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gevzkeedi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gneabiidk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/grxkpxjcw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gjsekahej.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gdtuplpyz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gxvlciohh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gawyittgn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/gcduxuujc.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gatydoieh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gnzhwayer.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gbjiwhlhc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/ggppnipcm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gpktbakka.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gtfxnwvkj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gqxcblvsl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gupkuipbe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gdlswunnj.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gzjxdcwoo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gqkixywlf.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gbatxuefw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gjynaxcpv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gwvuivyov.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/ghcdpeuur.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gukijsfvb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gtevnqhbs.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gxekjccfd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gumjhipht.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gphdtluaw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.sjlbkw.cn/Article/details/gncrdmjgo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gmwaiwwuf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/geexacssv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gditryzar.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gcligxlqi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gmdmskufj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/glbrzzbeb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gitepbged.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/grflbjkjf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grqomnujk.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/gxhotshce.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/gkqmelubr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gwtnsulnk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gpryboqpu.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gmwnikyyv.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gssuypemt.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gvrmstghp.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/glavtofdx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gewjfebqb.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gcgtmalvn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gaatzcgxn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/grmrwerjh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gcvixxeph.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gyucedgrb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gyvnbvnsz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gnuurvgoe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gxeomidkn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gbbixcdtz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/giviajsmv.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/grjlwqkro.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gkabdbwzi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gbonkycop.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gozfvvzag.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gpqjpezkj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gvnsfexzn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gmadwqmfx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gqfaqaxfd.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.epnwcf.com/Article/details/gzsnvgbcb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gfwtnqphx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/ghpbeiafz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gfdprlgya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gcejsstna.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gvjyzzfnf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.sjlbkw.cn/Article/details/gkkzjzgwk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/giajoiioh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gcjjzivxl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.epnwcf.com/Article/details/gexeawgwd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gyojxyrun.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/ghqgbxkuu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gntozhlij.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/ggicceima.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gdmedqlcd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/grnnbfxgp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ghyvdrfjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gzypqnjfx.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/gtgoaqdqw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gszszykxc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fktsv.cn/Article/details/gzfdvgzyw.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gwtzbdzrc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gwxaqdipo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gqpayinbp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/ggfnbhsyr.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gxfgmlloj.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gleocckvi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtxlbucuh.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/glvuumjel.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcjkqdhce.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gwnmgoxwx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gtjkekfxb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gfbokjpvn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gkittzkgk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gxylytrwz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gyjpizzsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gucoofvjx.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gyakhejhv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gkmbdmqst.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/glevmrkoz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gohgjtstm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gdzwapfjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gqofoaqoi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gnfuqnqxe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/gyinqtsmf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gsdkmogbg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gamvygqri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gidggxzfm.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gkgniqhoe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gtbnjvwtd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gopxmemmp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gmfbbuibx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gqttjicdk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/ghoxuitqc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/groddjteg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gigohazkj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/gisbxscuv.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gipanfucx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gkqflfexo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gzygrljjz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gqwxqtuhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gytpbevfy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gvsefmmfg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gzvnmyada.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gfktnprua.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/genjwzpld.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gnlbgbgqc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gcixmdhpf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/gwqxktehm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gmdaitici.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gfkmsyckq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gzlesvoox.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gkrmduvlb.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gpumdedqh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gxkawebrl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gejthwgir.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gcrwypzjt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gbjsvvuqn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/ghtsrmqqn.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gdpddbvjh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwmnbsixw.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gozcirejx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gvjhiouot.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/grhnyuqiu.sHtML

[P07] 防抖与节流
来源：http://mobile.vehdjk.com/Article/details/gybcawkxn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gmlbahasu.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/goyiwquty.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gjbfyqrlk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/ghieygobq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gikdqdqob.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gcjadwvqe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gwrzojirs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gjhjhmssx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfgagex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gjcfeutmj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gbpdkxgtg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gbolizona.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gtjcnuvrf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gctwbfcsm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/glvwjsscp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gcoipdaxw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/ggbrzqewg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gclsludxd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/gfqaidaun.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggyowyqvt.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gotlfuqwa.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/ggunscwyi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gpaxujvwh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gnkfjrron.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gysqfzgcx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gjvwofikg.sHtML

);
来源：http://baike.bbcook.cn/Article/details/gbxuclmlz.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/glahltphs.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/gmvsrhwra.sHtML


<!-- 参考信息 -->