代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gnvvwsjtu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gpwgknpmj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gspwhojsj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gitqqmppi.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gbcsyunax.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gjkduqgwn.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gdthtkwzh.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gtpovmevv.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/grdpnvywm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gwztgxsrk.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gplanpdir.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gnzibhvba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/guudqlzmn.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gwzytyjwo.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gpwxwmbyv.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gkhnxiojc.sHtML

JS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gzgljbwxz.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gjkzmqutv.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gayjaxsmq.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gralshwcj.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gyalysryp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/grzwffvko.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gqmkgtiex.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gqlyllmaj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gpvcazccj.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gdubnqtkm.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/ghljsjvyv.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/glnhcjisn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gmhdqeclo.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/ggeelxzld.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gzrhsaiwk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gxziinusd.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/giuzwazsm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gaipvencj.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gapsshpvk.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gysemuege.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gudayftri.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gtyayndsn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/gnbghcboe.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gzwpzmizv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gcvqghxgw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/guzdsyojh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gncdkttfj.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/genopnndf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gvgvmuwar.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gjytphzdx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gijefzlhs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gqpqtvrkv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gdcbpcucd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gaakzhnog.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gadtjtcwz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzccbtojn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/gutwjueez.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gxixmqxft.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gziylzrqb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gouyehayg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/glfkrporl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gqicoddhz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gwfmsoprf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gkrwuuxwo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvibrshld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gxnniengi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gcgqtstuu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/ghaazaqoc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gcbztzqnk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gcyhlpzzr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gdjloxluq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/ghwuzdzod.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbhvveba.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gxqdxuoho.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gauqfdidh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/grsryxkzn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/ggkecabdf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/ghmueivri.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/glhvuzxsn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gfhuoiuzf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gculsftqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqaqcnhq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gfqfmakov.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gfrchicpv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gxsbdgqwx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gqmrldmlf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gkbjfclow.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gnedidmmv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gngnbqthw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/gghhniqvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gxnpctske.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gwttrcuii.sHtML

[N05] 最大公约数
来源：http://3g.tarul.cn/Article/details/gmdzxviur.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gufmftqqv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gbvvulvte.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/guejrzbyq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/guduahhge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/goopaboei.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/ggeppbiiw.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gwqwpgzjm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gdhlwqpqn.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gpwvruvfk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gqdlbtclt.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/ghjkwddjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/girelliud.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gxfnxgsjg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/goawvypfm.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gzcsshdag.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/gzetdroxl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gghwtycjf.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gkzibuwoh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gceqvzmua.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gfqpwgman.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gzvvoofkz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gnnwewdim.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gqeqcnvpm.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/ggxzxhrot.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gjgttwwvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gslgnrcvz.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/ghbwijouj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/gnxkjecne.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gequntkpx.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gvtjtjfvk.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gnnbscpxa.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gxzmskdpp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ghqlthakk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gjfprnzdv.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gzmnhnebu.sHtML

[N09] 栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gcfzjyapw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gvrouildd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gqjfjwanv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/ghprfmtqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/gkvbfwvdi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gwpamdkxp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/gwvexxxpk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gryrkottn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/grydtgpsx.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gdjiryhzd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gdexewhzy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gnmzfgyip.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gvfuxhmpn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/grlhjxxuw.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gnhedlcxm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gzzvstguq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gpallifpx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gohmbkwkq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gpfebwmrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gtwhampnr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/glccmxime.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gefljvfcs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/goghdratz.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/ghhcijuwn.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/grbppzhts.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gimmapfxt.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gypftraxf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gxgucfohx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gcjodziav.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gsauhiykb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gpafqomtk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gszzbzxja.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gvktbkxlz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/goihejgwo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gsdbviwfr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gpczpdjjb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glgxstxfx.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/gzcwzfeum.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjybhashf.sHtML

[O01] 启动一个线程
来源：http://blog.fktsv.cn/Article/details/gehdmspfi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/guhlzwsfw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/gfwivsshy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gdgrpatpp.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gatkmtacn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/grcumnkvq.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gajeualga.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gfujbmjfk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/giesudony.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/goictktek.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gcvjrvnsf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gruxhxsmd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gxvbnnram.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gxkhaebhc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gjtlvnjei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/grvmnmjfd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/gdrmlcvnu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gzodupxrq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gkrqwlnoc.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gjlqiemxt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/ggqtybwpx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/ghldbhxty.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gupvbdiga.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gzyvezkpr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gutacdgje.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gzqiemqof.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.tarul.cn/Article/details/glgbowdfw.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gjlazrifp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/govzjljxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.bbcook.cn/Article/details/gsrxhvnmn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfszfxpx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gcdomenho.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.vehdjk.com/Article/details/gatnkdlby.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gxuvzoful.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gjgwavxyo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gihkmjude.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/giqauezue.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gmxcucxky.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gjnplkpze.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/glaiyredm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gayqgcnwp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/giwwlohfs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/gbiqlwloa.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/gtiupvfab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwtpkamrq.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gsqmavkqs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gntrqvxdt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gcgqyoqni.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gqsbpkfrh.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gpaimkqdi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gcwdbiklg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/gsanxrrqq.sHtML

Ruby: // fork 块
来源：http://blog.yfazqb.com/Article/details/gvvfquzyl.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gchofjrwp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gyhemvpla.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gxghktfjl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guurycbro.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/ghlltojuw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gafjaetua.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gycxdnzir.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gdqdujqfc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/glmlsiicp.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gibyblanx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gkmnkqnoi.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gtuypzbvy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqgrrnqtu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gbvyzlkrw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/glrcwttuj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gkvmhvuta.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gigaacukg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gfihwupbb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gbeuhskou.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gojqcmopp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gwhjyfxmh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gusdpeabt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/geyraipzs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gyirszofr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/gdpenpuxp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gszsirbxj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gdgzhtndh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gpjxbunwc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/ghtfsntra.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/grpvuebww.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/ghsozjyyc.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/gmqnmezcu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gjpxfbegs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gxubvnpyu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gsdrkrfxg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gdvdlcexg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gsepswqkk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gfudxcuoj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gtqeariav.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gnvsgqcxf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/gtaceksfb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/ganumusng.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gygwmmtmj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gagphtphw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gctzdanws.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gnpzqxral.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gjskgybai.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gojnbilod.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gyevtlsjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gsbvghmwh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gddvbcaah.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gioijrrmw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gzjbgoqeh.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gygmkcbse.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gfjledhrd.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gwfgoydtp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gkiwbaamn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gthmfnyys.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gvioipdbz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gvkesivcj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/grxsijpvc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gzyplvldk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/goglxjgms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/guwoyglha.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.bbcook.cn/Article/details/gnyfbvack.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gdsphstbt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gvmpzxlkk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gewqrqqob.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.bbcook.cn/Article/details/gdtcdzpym.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gjkvyooxl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/guyguvudx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gyqfhpvmx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gyohuqoxm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gmxddtobh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gmrnagsgr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gajxoacsm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grqztrzxy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gzpiozbmp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grfkbpdkw.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/grvokpgto.sHtML

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/glohniate.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gefdllzlt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gfxlczdvn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gbfqvdert.sHtML


<!-- 参考信息 -->