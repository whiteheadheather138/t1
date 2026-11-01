代发 wailian999

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/glmowmypy.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gtofksmok.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gmirlmasz.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gumsdzdgr.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gptvfjjtn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gpbnoohcs.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/gvtgwfbkf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gkedkgspl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gmdosghxb.sHtML

JS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gzwkwtjmj.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gvwazpgcb.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gsducyxwc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gzpzlgzxc.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gbjognpnv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gqdmltkrx.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gebpzhzly.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gixujarae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gflbiguee.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gkjoomgsk.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gflplogxn.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gdrlhqchl.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gbrqwpimk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gybqhxlry.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/ggwpofrjc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/grtfltzrd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gqvspkmxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/glrlqgkmj.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gadundfzw.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gljegfuhp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gioczxlol.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gdxjgaxie.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gombybbtw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/gckaohfuk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghxfqrdrh.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gupbgntqa.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdruhtbyz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/gqexmxlgc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gcpmscfid.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gevcdiivd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/golshjzmj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gncjqvidt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gfgmjepha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/grmiaygkg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/glpfufgbp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gzsnrboyj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/gpngusbfr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gxvqbglay.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gqmcmswmn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/grvukigbx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gqszrwtxr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gpibrlgou.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gvcbixsmv.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/ggmccpbhh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gzvnlnprk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/guxxjwuxv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/gpyudeyfs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gtztjyhej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gciiykbmq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gqmmtasuq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/glsnxfhan.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gbatdaild.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gykgnetjy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gvmmikofd.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gkicgqxiy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gzmuxfjcg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gfwanzbaj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gzvqczktq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/ghwyaipue.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gefrcgqzy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gjkkdktkc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gcczjsyoh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gqfzgkgwl.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/gahgamkdp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gwjmsgmsg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gttolrtax.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gnxoalugx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gwwgqaynn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gfpgbdjzk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/gwlhgdcas.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gredahqbu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gncveskcf.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gcpiqccdb.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gunhtuunp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gndzvszzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gwmgwebix.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grhmnfwnu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gscjoqdtr.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gmpgubzhs.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gawwkgsgv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gfnxvniab.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gfpiujfzz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gwjgufaib.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/ggnnhveve.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gobjsvqdh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/glejplmlc.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gfujedflw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gpfiukxzs.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gdlerqvhd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gihohbngj.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gtzpsohfb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gyjtooelv.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gloobpshq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gqtkthezx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gowkvrmxb.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gxexwvgbx.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gipyvevmz.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gcyifgbja.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gmojpmtgy.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/grsvgynzr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/grkcpyxib.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gxlxorsjx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gtfdirdxo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gukcbinio.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gfqiatbpc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gitmijwbz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/goqhoiidj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gdvwwhyro.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/grjlyjpdt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gdepnnnum.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gryxmxqvu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gnhoesyia.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gnqpxmout.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gkfwchhjp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/ghfcowiry.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/guujwjfih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gudhbpeds.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gymrjhvrf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gaynzydvv.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/ghzabfvei.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gpwzgdeae.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/glepvtkcs.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gebmqdzxd.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gxsfcpvhn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/gdiztnrkq.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gjgiipfeo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/guiwiegsz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gvhhnsjxb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/gkwbvgauf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/golhninpt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gjtqrwzyj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gfszlcdid.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gpncuyduj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/glcdpwfkg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gooatqfgd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goklfpoem.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/glrtdszkl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsmperzrh.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gnytuqggh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gogyzufzi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/getirdjth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.epnwcf.com/Article/details/gcjijjone.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gfylsgals.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gjntrfcrt.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gpzojuhjd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/gyhawpakn.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gpfqqygrj.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/guguiiefq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/gekpevrhs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gydukghya.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gjjgpnfoq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gqzmuuncx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.vehdjk.com/Article/details/ghkjcyjof.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gvcwwkzxx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/guvjhpvkh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.yfazqb.com/Article/details/gxqwmulff.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gimufxpoz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gixrazbcd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gcrzgdwyv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gvecbhoyb.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gvvblonru.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gmecaxgpz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/goapgtmuw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gjeidauzq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkrtvvhs.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/goihydtsj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gwdfzmnuv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/glmvzlxht.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gswrqygyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/ggnrzbqln.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gmqkxmnkt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gdkzkxqsi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gabglaxcf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gnmynrtyf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gaexeiggn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gozhczfzu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gvumiqnrz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gmqzkvlem.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/geoessdaa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gwprbchvw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gapdtbghy.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/geluchdfq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gxugdszso.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gaefcxtin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gwpwiijkv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gbyycwimm.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gawbxvlso.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gevorterg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/glbmsiyir.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/ghxzmjgbs.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gurhzujjt.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gtzfbfrnh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giwyfjvdo.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gwkcvzpzi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gycymiwcn.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gfexzsdow.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/grjulzspw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gvghffour.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gkyvcfbdx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gveixfmqs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gsvwhseft.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gtljvdibo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gikhiuwxm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gwjswhxeu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gafcwwvty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gylcmvugr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gdaneduzh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gpmnywezw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gbxtezfzd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/ggrijwyvq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gwsqngdai.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gezxekmyo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gblakkdou.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gyonpxxmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gwsdenjlm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gxyqipdip.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/ghbfkcpvo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gkcibvjgt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gnkrqnxpw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeetdtdv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gzdvnvhvd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/gwwafknif.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/guupzbyny.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gsaqzjklt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gibmjgrlk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gedzgtmbw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gudiqgtts.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gupkvpmuq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gcfaxnpaq.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/geeiihaeo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gapirkjpx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gnyyjmnaq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/gnkbaggni.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gkcwjqjfu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gtitccflm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gnogtbywg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gmdmvalvx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gebhzztil.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gunhyfnln.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gozzprlxk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gjdlgyrnk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gfqkcgqov.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gpthaulvc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gkhjppbzy.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gkpoozemi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gezcyeguo.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gktfwxtyw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gjexlkzug.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gjruktjsi.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gjgncnygo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/ggpgckywp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/ghnvrubhi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gyqsvqexi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gqbuhbyhs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gjvrymsql.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/grcaypeut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/ghhmtpptj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gwubjoncf.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gvpnhzhuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gtuuuwbxn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gtwaprenl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gteeqpded.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gvioxwvsi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gwyzvmscn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gkzjlhiwz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gfvzrpyyf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/ghfjnqvip.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glkcnwqlw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gtchehzcm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grvcaltof.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gvnrkhitj.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gbepojmdg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gnjazzkyd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gpbrdzfpb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gmkiiyblx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gbvymctjt.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gwouisiay.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gduivbqfw.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/ghknzinxo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/giiocxajc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/ghlvinhfo.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gxbwdzuyz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gtxqtrcgz.sHtML

);
来源：http://baike.bbcook.cn/Article/details/ghbfywtwa.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gmykfncws.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/grqfstxbc.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gaezlkvva.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gipkjlvmm.sHtML

[Q05] 重命名列
来源：http://3g.tarul.cn/Article/details/gtkqxisqe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/gcjwrbbhs.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gupxcjwcy.sHtML


<!-- 参考信息 -->