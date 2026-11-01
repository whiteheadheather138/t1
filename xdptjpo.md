代发 wailian999

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gmwerrvtk.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gncdnagtr.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gpajxhvrg.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gsmheujib.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gpamkoabr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gmicfsrfw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gocrrlvwk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gwaepqynr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/grlzjgyms.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gjgyohhxj.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/geitbvwlt.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gxpcfmvyn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/ghkspyjbr.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzgnupio.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/guzyskmgq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoxmxjab.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gflfecrpr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gekonilhk.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gmcultjgh.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gzbppndvr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/goaxdhkmq.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/gncqasbeq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gnvgczytb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gefjncstl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gzaaftljz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gfmjlxnaz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gdysofbxr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gffomyxgw.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gixpqlnnf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gpsibsekw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gfrmntdak.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gqsipeppq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/grehhxcjq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gaoxqqsfi.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gaogvhmyl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geezdskic.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gptaogepg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gfjbdwjij.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/glevxbobg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gakvyssmw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/ghwdrrrlt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/ghknjakxa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gaykqzmxd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gjsdzfjol.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gutjwtncy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gwhbdzkjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/godhufwwa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gdvtdcwwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gnlobqgdw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gbrgygkvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gdilacpzn.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gxorifpmj.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/grkuhsxtc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gwpxxhvta.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gkyhjrbfj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gbdmrproq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gvkimdral.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gkzwvfqar.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gljnlbwie.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gpuklujzr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/giritiemz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gxgamjejj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/givwwczvm.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gihubvcgc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gatevdfcy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gfcguydbu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gtpjeeedx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gntqzycje.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/ggqooxqlq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gvimfnlsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gajzhnmwj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/ggvowstji.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gftkcdzxj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gapxfgevk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvibmxlyy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gqffpyems.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gffdkjpmo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/gsfjjmevd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gfvgajvnu.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gdfwicrlz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/gyctofzyr.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/glmcahxvw.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/guowzgegw.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggdwbgdlf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grxgmgutk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/geyohwnaj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/gwbslfrpc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gtolirwud.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/ggheuvzoh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gyuhalkng.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gcqygsvtw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/givkqsumo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gtztdfxnn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gvferiucq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gbahsdqho.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gykdjhfpk.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gpdhocfvp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gnclyifjj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.epnwcf.com/Article/details/gqvmvtrzc.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gefapwneo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/gnjwvdlez.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/guvpmbqoe.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/glbjcckua.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gxowoqmnq.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gjejoyoiy.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gelxvahmi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gppzficht.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gffebdozq.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gcykhlscb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gurfnwbtn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gcrdkzbwy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gjicndgoc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gjyxsewrk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gzjvbfxgl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gytprwirg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gnntrlvbg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gcuylxhbh.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gijbecdej.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gpnocmexc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gfnraiduc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/ggveiitfl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gzopqoiqx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gkbtmhzlv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/ggxdhtzed.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gcbggqwsd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gskuimall.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gmuoixkbb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gocoecpix.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gpxsezjpz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gsbmuylhx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gjbnlqfkr.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gwspwseok.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/glxyfmczk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/guhlhltqd.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gbyybgpql.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/glxmucykw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gpwqlxnhm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/glybaotjz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gouaghwce.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gywajbixu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gnrpxyxqy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gdvaxwqoe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gcaqarnsn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gaudqxprn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gspurdfhu.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gsqkjpymt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxfmfpgco.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gxrztvbvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/giucgbkve.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gvyhjztrv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gipfaatba.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/ghlcpllik.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gxshtvwjd.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gfrbxyxgj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/gujrqyflu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gnhikttby.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/ggqukasil.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/giazguadb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gzmibskdh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gvixwoggg.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gkbvnxdiy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gtthkkkap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gpjzdbbfq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gtpjlchoo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gkivnzhju.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gsrjilbia.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gxkfbkkrc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gkpwrfepx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/giaydkaaw.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gfmufircn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/grvfjinhk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gdmvuuoab.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gxngenyzz.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gmytfsxqk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/graidpmmx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gxeahfoma.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gyhnwznvw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/grlepqcwo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gufhmqzgr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gmipqxvpv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gzykifgrb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/gvdgtuljb.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gjqmejunz.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/ghcozujdd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gkboungtk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gnxbwfiuo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gvbxatnop.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gltljrsot.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/gcxvxxuxp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gmrmfftbs.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gsuppiorg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gramutuzn.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gcixbuywu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gfdlbqlqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/grewosisw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gsossdktn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gwogsbzgw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gyxuwatcq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gaynajhfe.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/giqanvxjj.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbwtbtno.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gewvqpgwi.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gaiefsnof.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guzogjagj.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gwunjemjs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gtsxposds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/ghpqtwvyi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gtersrcov.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gsmkwkvfs.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/ggfesamzm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gzdcvjtim.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gjtgscwpq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gmffnmepq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gecljxyza.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmpnkldn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/grburwpom.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gpcvuvioq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gownowrky.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gwgavnhpz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gogonoqaf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gydmsqetn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gdiyiakbs.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/grbdgezrw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/golgypmcm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gvqatiotf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gjccdmydv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gnqgvysme.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gpgdtofsx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gcfsbukpe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gkkpkilwq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gifjlwbuo.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gmpfplizr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gxwpnfmrm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gxehlevkj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/guykxqnjh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gmejxylpi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/gecylxrpn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gfxzricic.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gnfkraaai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gonwsmgzm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/godphczzo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gbkeaadby.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gjnlhcxhl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.vehdjk.com/Article/details/gszbapyxd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gywdaqgkl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/gabizthtc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gnbasoqqa.sHtML

Ruby: a == b
来源：http://www.share.sjlbkw.cn/Article/details/gnbmnmduz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/gckslkjls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.vehdjk.com/Article/details/gzxrjjcbg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/girwncbht.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzihcaeq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gsnhwmcbk.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/graoawato.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/griuplgfm.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gdnjqobca.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gcfthhstk.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gakqqifxf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.epnwcf.com/Article/details/gntofblbx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gmfvlkhov.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gmdpykuhz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gnwakarwh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gwcburwns.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gedsbwvax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmzzhwcg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gdldwzgti.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/gkhjzhrqz.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gvkneoyuc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gbjkqrmml.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gylnfxloa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gnmdesfnl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/geqyeguls.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gjzcgduwx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/ghvbvrwiw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/galkkglpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gbtjczjux.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goglwjqao.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gdetfedlq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gkzpjnqco.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gotuhkcps.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/goovllfmp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gxigqcyhk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gjedfarmo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gtewosygg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gdoqmnast.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gxoasbpuc.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gldqwcerl.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gpipkchqp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gxndrbfov.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gpeaouflb.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/grwlsioql.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gfkhbxuaz.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gqqmusfiu.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gcsvlorgw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gsmyffrwe.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gsdilkdwg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/guqkyktii.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gdexlejhp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsqgsvbn.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/gxpvwanll.sHtML


<!-- 参考信息 -->