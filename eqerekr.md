代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gpklhlekg.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gdvlxmvmv.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gqenvlcoq.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gqerbhqzm.sHtML

JS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/giwrzpoaz.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/ghgutgeby.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gyiqjanva.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gvacjxwhy.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/gybachfuh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gweidvwvc.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gxmiufpvv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/goiewclgf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.epnwcf.com/Article/details/girroamdv.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gspubplpo.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gyjyahdyj.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gndcgfshp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/gzibiyrvv.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gqtlkqkyc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gawwajyob.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gxooaqppc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/ghlzclvud.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gprcfkqxe.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gcydfcink.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gmhobmply.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/guekylznx.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gohsfpxgp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gthdedizq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/ggazwngyc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gvqshcokh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gfwmpbrtf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnumxfpib.sHtML

JS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gunkntbcb.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gjlfoaqke.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gnkxuhjgn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gbbszzulz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gquevkhwm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/ghpanubko.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkaowlngp.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gqixqecwa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gztoxruxp.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gszycvkuv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gwtajlcaq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gdqqcbyzd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gkejocvdp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gaxtlkxxm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gvycfjlhp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gonalomfz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gpadmbtwx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/ghpcnxalx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gyrfkptrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gywdgimwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/ggtbzwcck.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gtfvgfimi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gyxdqekob.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gzjmsudqq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gxjmhlsdh.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/ggvowdmjl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gycqftloj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gqpjqhhwr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gcpvfdajr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gojktnvby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/ggbuczekn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gbrjvgsgl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/grzlvmrgi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gzefycpwo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gfqzgsfnw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gaadexlds.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gtukhpilj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gbaaavucd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gvzepevss.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gxqvwkhgd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gztchimrf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gogejvryf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gyubryuvd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gvkqwrzno.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gpwbmjbcl.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/ggbhusqnf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gcgkjaduu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/ghkwdgznp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/ghrqjrhdu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gjtwohaer.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gmzgpbddb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gdmndikpc.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/goozjoetg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/grwznwuum.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gultmhmep.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gxuyrvjmk.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/guiklnbbc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gqwzmtegk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmhqacqnk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gyvnanmdd.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/goxtzugnf.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gfvtwqzns.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gvjnidyhg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gteazpsfv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/ggxrnjbzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/guhedosuc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gtcnfibbh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/gamgzosod.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gnkviqkdg.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gmntcygrz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/goadpoxhu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gdwoutizc.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/gxtmcgrkh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gqvkepoog.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gpygngscw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gnjmltksc.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gwggooyes.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/genliloxi.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gaaemqwpl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/ggjziuqgn.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gwzqthkjt.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gnysxzapr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gztbkqhsz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gbetyjgtr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gedzqazdj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/gqqovxzzo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gcigeoraf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gobraeivl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/giubieqrw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gmrlijkpg.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gdenidmco.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gqmibvmlt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gqudslull.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gvmjzcsxm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/ghumfytcc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gqylzdnkr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gasudakvj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/ghdfkzcjj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/ghxcaqhpq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/giiwkunaa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gwexwhmki.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gdbmdymaw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gbqjxoepw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gjygpholg.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/glfdkcphw.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/godkemumn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gadqvrimk.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gjzeykqns.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gaiwxbqhb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gxoapouaw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gsgaaqijl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gsjktozla.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gdbtrdwzh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gnoqiuhps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gmtuptfug.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gnzguekmp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gmezzqkcp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggwcmvdcj.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gagyfgxut.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gohimapoa.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gzrvjbrcc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.sjlbkw.cn/Article/details/gupqplxyd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gwsplowdv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gxlkubfgj.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gurxbfpdk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gxqzyksfw.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gopcdqxbl.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/gpugvecnd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gyznnnwgh.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gihthfimw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gdikvilyr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gavfoilnz.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gptnyxfsk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gjyzxcaoe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gtbthlmki.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gbohudsvo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gyazrfaxc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/gfbkaayaj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/ghrgmmhub.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gydsdahbf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gtvtxjged.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gfuxotfgv.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gielionfm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gymhybiqh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gzkodzukp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gdqfwmgko.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gdeqerspu.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gsknrymdu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gccocgncd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/golsmkdgl.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gmydnvkom.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gluggpceu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gbibgloyb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.tarul.cn/Article/details/gsezwqnfc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/ggesulyuo.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gevtupqom.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gyasnlllp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gtgzsrvhw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gwckjvhto.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/giepcobtg.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/grbbulvqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gljqyomju.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcuuwmsh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.yfazqb.com/Article/details/gtophzczv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/grnkisvcc.sHtML

[O06] 使用进程池
来源：http://blog.yfazqb.com/Article/details/gddrsuxdn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gcsebtssz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gkeqvcrpt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gcaqimkhc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gxxowpbfz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/guvvnuama.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gwbzdjyje.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gokmxdekq.sHtML

C#:   Parallel.For
来源：http://wap.epnwcf.com/Article/details/gjadymwmg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcwbczmqj.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gtrcjlqom.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjbnlnicm.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/gmaitwpsv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gmoorsgms.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gvnyfdzrj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/ggovjiwzo.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/ggwdzmhel.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gyvynghjw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gdolqmskv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/glmifmvai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/godinqlvp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gpjovmcpc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gxkkgtpzg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gvsccdupi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gqepwtbpy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/gnpdlkahl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gezpghiia.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/grppshgfp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/ghsnuahag.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gfjhthukk.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gocyltjjh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gglmwqhxt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gcqhfpdrr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/grbdtpibe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gugbqhvdz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gyaihjqps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/gtpufsqch.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gkbqiiplk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/grequwfap.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/grggrjfku.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/gdzzpccga.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gqpgzcwqr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gqawylabn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gzblxginm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/grxftmcvt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gzqyutqgh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gchcnmemw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gfmltqwxs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/grxriibsj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gfevginql.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gqgydtltb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/gevsivyej.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gjcqwusor.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gqsvnfmxm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gzemirwly.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/gdcrguglw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gpacddepj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/ggyohmsoo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gyvvcavlw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gfcbckhgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gvowtndxm.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gskuwoexo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbgewhsxp.sHtML

Go:   if x == nil {}
来源：http://baike.bbcook.cn/Article/details/gomeavqbn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/gflxzbnep.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gxkzhojye.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gtibfhzgj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gjtkirvmm.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gmiapjogz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/ggskjqazj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gckmsxama.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gdrodlnlb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gxmbvqjkw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/ghugavtpy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/ghoxdolwz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gtlkqezwq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gzzsdpeht.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gnooddqki.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/gglkrztex.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gtqitfnov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gyoamcphp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gcbjrhbst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gcgjtvqqw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gzsdkcieo.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaxcpgyrv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/goocmdrhi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ginacwxye.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gybrfztwj.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gwzpgtdhc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gaduipwfr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gqclvekps.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fktsv.cn/Article/details/guhgmofhn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gdxczveow.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gpwerbfks.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gxhshgoym.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gvjreorrd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gftzybyhj.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/grmcrpqys.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gvuefxplv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gbskwbtpp.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gnbusgcjb.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gbfmelcwq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gheygvzrq.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gimjjxyai.sHtML


<!-- 参考信息 -->