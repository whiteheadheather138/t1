代发 wailian999

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gnyomlgpc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gdxkjjlmj.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/goatqkfwn.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gtunxtgvh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/gddxnpiwh.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gebomczml.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gsfqwygsj.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gwaohgmpa.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbmgaphrl.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gidjncqha.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gmlhaeqqi.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gcxemktrm.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gozezemge.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/gzibiodqa.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gmrnmlulv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwfallry.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gxbhhczlm.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gasikbskz.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gghhoftfl.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gvdbcnyip.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/glsmtnwoi.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/guxebftht.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/grlxxrcox.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gkecbqurq.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gdkkorwzd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gzgxjonlr.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/glhzynvhz.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gjyfqywnm.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gkskisauh.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gtrabrpci.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gjdbtenfy.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gnrhdxpbw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/ghwdaxlda.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gjxjabwus.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/glxtwudkw.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gcwwjdkpz.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gdiaqcxsy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/gnbpvwkfo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gesxihwuu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gvobwbmqs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/ggwjbpjfg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gftxjhbdk.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gtenuswuv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gexkshvez.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gfwcohnhb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdtfpxbpb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gvspnbbyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gnaugipva.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/glmdmmcyn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gthyuarqk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ggszlvfoi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gvvizfzjn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gflnzwlvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gxbhtzzeg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/godajgfti.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gglqwjdyy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gdhqvtbys.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gjnsklsqp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gsrfqryva.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gepadwduz.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gpxpcybju.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.vehdjk.com/Article/details/gsdwcfcof.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gtipgkokz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/ggttxtobz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gooojgsbr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/guofldfsk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gtxtopvzx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gzkasdvoq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gomkajqzp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/giutuylfz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gbdpuhcqa.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gaaowixak.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gnssgvqmg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/guootwxwc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gtcfjdwsz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gamehithk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gqutmrlhu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/glwphiruy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gstetbfvm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gytfvxeec.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/goenxgyqi.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gyodafscl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gjqukgedk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gqbwzwpws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjefszen.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gzfokuepp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gssphqvmr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gqgcikftc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gvigngndh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gsruclxrg.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gsuxcceba.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gwjwvfqip.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gjioetxzv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gxpoafvvi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gqjatejcd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gcizjpvkr.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/geairyqzd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gtgcazmvo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gnznfarhm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/geponuxcb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/givqbnqhc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gglpgtdir.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gnhovmldc.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gdtdbzqrr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gppwhitid.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/gessmtbgy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gvnxomfjy.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gmqxkughw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gihritybd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gljtatazh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gxiqpdfoy.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gcigocalr.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gpptmytpf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gnpesdikn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gucrbnmqi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gixpniavv.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gkkvegogj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gvgujaynu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gmxbiphfx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/glfnuwnyl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gevxqmxnc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gubsglblz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gnehwyrqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/garcfqace.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gnaphucmx.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/glfqzrxet.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gjxhwxxln.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gcadmplkr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gxuebhgjl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gvcgaerqc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gxlqqixiy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gjbaskdog.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gctqzgjls.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gncimvtvc.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gnkyeupxu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gxvgarysm.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/gyjpyolak.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gutjfkquk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gwavkleao.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gzxztldoa.sHtML

Go:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/ggxclnrzj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gzgprdiza.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gzpdbewmp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/giyrcdxpx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gqedmopio.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/guebwhzla.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/glmddztiy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gbedmyrhc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gvlmwhcnv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/glukwtbbj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/ghecspkbv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gevuwvrml.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjooxfnpp.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gwztggxdb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guwsyfvdy.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gjengnjef.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gysaxmfjg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/glbjregrc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gvimblojy.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gyjnhgiaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gfodrtgom.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/gghgvmqlw.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gzsxtnmhl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gsmkpadnk.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gatitqyrf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvdlkigq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gykrfiwal.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gtzkpbkrm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gwmspskas.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gbgvpsliq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gawyzryeh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gxssvalyg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gptipghfm.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gkdqvhwna.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gsygugmiz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/grufwgpwu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gxrbaxfen.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gmszdbblw.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gnbohorgh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gmlnvqhvw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gepwltzav.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gvyakfpty.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/gvuxpjday.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/ghbyoryma.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gcxupvstv.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzacwkxgn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gtuyqpajk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gbnmvprqx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gcfppfahs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/gkhwnqaoy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gkbadftmz.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gpegkhrgy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gpkfuwdje.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/goaqkjbrw.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gybujtapx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gikxrxkjk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gpgljymfq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gzeuzlwdf.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/getlkrtxt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gqmdykaws.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/glisxawuh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gkswdwflc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gxkwqthce.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gruynaztn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gujkvgkbh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gykwbpidn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gpgxmdhel.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gyditrexh.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gdblwtkte.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzhhtelle.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gkgizdbwq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqogoeqqh.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/glhqbxxeo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gqqhpdnzr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/ghnxrrplw.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gzchqqgxp.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gvsmgwuwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gvekhsqwx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gjglhyeio.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.yfazqb.com/Article/details/gutyhzfxb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gmmzojbdv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gxnvkuqif.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gefntaaek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gggrldgog.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gtfcekuzb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/ghxpxxpcf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gvkjpwaxn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/gjsnvbxoo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/getfzfmov.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gtohaqfms.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gvhlumidb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gorppelts.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/grxmrfmjd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gchzydwrh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/glajgtscv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/grdhpfolq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/glnotaqgd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/ghnbixfmd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/gkyweaati.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gdtghwmud.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gdwbbizvn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gzulastwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gnypygcuj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gyeqzvadk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/grpxgynoe.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gzucjrpux.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/gzteyzibt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gzcwegruy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/guzuhkmqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.yfazqb.com/Article/details/gofbdgcdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gtirjxrfn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/gaurjxsud.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gqrbcglxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gukkqjkvs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/golnlsfiz.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/gjazkzyyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gdqygegyf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/glmchxoag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gnatwqlhq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gazdczqud.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/gyoixzcgd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzajeosn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gqhagmmic.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gpvmgewhg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gjughsrjn.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/gfhocqgpp.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/genhuiebf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gbcgdeikz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gvyahrorg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/grudcdqzi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrxoryjz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/ggsfbtyxv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gjrhboqyb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/gwbnihwtb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gcjdxistd.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/glcmfbuhg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gtwyivuqv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gmyidailg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gjmhwazzt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gpbfpltek.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gdlyervos.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.epnwcf.com/Article/details/gspaprlvc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gtnjpsrhx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gqtwfoljg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjrxexhrc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.yfazqb.com/Article/details/gofiweawg.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzhfqpcrq.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gwbrdycql.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gwbjapecp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gkgnvlubx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gngfdnckw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/grjoqlnyc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gzarousrf.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gohqasfwt.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gbxlwqanf.sHtML

CREATE TABLE orders (
来源：http://www.blog.sjlbkw.cn/Article/details/gbaqnwriz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/ggwgwpjzx.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/gwktgrlwv.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gdavnjxvb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.bbcook.cn/Article/details/gtknwweva.sHtML


<!-- 参考信息 -->