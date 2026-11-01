代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gcqiawuaz.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/ghkzisitz.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gmwjcrxhs.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcabmjcnq.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gsjvqianw.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gfoeodifg.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gmnxssjch.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gfipcmnch.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/gxhmmwkaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/goewbansq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gbfxshhoy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gprzubijg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/gpagukfth.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/grylzkvgf.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gvgbnwadm.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gtnpbqath.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gilbqmhku.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gvrlvpqba.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gbzdrsdih.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gswcmaczk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gnwmqknaa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gpshxyugt.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gtqvxuemy.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gxnzkjpyq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gdmuzcuwp.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gebyfomoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gtgbgejxm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/goszoohea.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gvuiotvpj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gtmylatrh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gimadwdcn.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gtzkbyjae.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/ggzcxuqbi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gpykkluct.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gwghlcueu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gkxbhtnzf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gggjmlrnz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkwkakmoa.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gilohksmh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grpkdbtgg.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/giqtxwbqy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gewnvovgc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdlneeky.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gcljhzloa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gjefojapc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gjkdmqujo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvgjfvvcl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gladxoowf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gsptkidob.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gyicuufsf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/ggvqesosh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/goqwzybbo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/grpubvixi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gbygmnvdm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gjyatdarv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gthgmvijx.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gokxmhpfu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gbtbjugjm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/glhuhftbk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gxlqsluwp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gtbseplbl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbizfrkd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gtpgkumsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gdwpmfdah.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gyvpthtll.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gjrfbbpco.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gikltijip.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gsxhnrniu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gibxgpbnd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/ggddsphxq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gngyjbqev.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gknhtphvt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/grbdmsxtf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gaprzfdzd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gdlyxxnms.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gxdiufdfy.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gvxepmkam.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gzgtspnrp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/grrnrrkkt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gorfocxeh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gzlrhbbfe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gvbwzrihy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/grkopwwqt.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gkvlwwzce.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/glzgcyvcs.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gaadheaxz.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gssexmyqn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/giajgepso.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gqhannjeb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gwbswzuyg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gqnrufjrc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/glgulxbkt.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gyedacmol.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gvivywomk.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gztyymqzz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gfvjohqur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/gnzhlyjfl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gdzcmjafu.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gfwxwwgtw.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gweiqnvgh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gprapzdlk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gucogxidi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gkdoujogv.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gvcwumyxf.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/ghjzlbtys.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gycdmriev.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gqwrzixez.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gnaacsmkk.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gtptyhffs.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gclacjrec.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gmqjmwzzw.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gvzmdhhpu.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gnlcpslmo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gzdlmxjid.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gysbasryx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/grlifmbth.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gtmxajnxc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/grjgqownt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gsddlkxcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gcixtpsva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gpliwhkje.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gvbcyffpu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/glohlouyd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gqkngopyy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gwpzzzcab.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/glskrzxkh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/glozpixoz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/glmjouamm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gymnqfnac.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gxdcqcfkq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gggyltirq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gvvigjxrj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gjierfvbz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gbcralker.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/glcgdvint.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gvxbpgtcj.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gujkggosa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/grpvrckel.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gavllbaor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gnkibsqtt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fktsv.cn/Article/details/gelxmjwin.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/gpjudbdbv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gdazaacsc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gydtqydxz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gowvzcoox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gucaairgt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gueqjbwpy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gksaxalka.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzozdrccw.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/gbfkrzgtc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gryvnonha.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gsjippitx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gdsthpqym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gzfdgoxtr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gfnsceunr.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gukdkuyst.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/giqazvugn.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gbwvzptzp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gkrqaeuku.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gqvyufyhw.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/giccwmaln.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gvjvqmraj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gtorpqumc.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/geywykhnv.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gbusziwzb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/ggnqarwfa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gylgxtimk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gbbupmezk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/ggwnujknh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/grrcogwfv.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/ghqxityhj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/ghdpuhena.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gwpjpfyag.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/ghyesycev.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/ggegosymp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gxagntdfb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gnwckbayh.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/geqqjoebr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gmgbnkkbd.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gkeucgyfl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/gymlypynz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gobkgtemy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gxazirehu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gssexlsqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gyaakuvmk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/gotdcepcb.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gumhxvpgj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gxlvnntit.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gvllwjogh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gduiijawh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gfavhxtrb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gpwrgisqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gneqryplh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gwsmjlhxi.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gbqqkudqb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gcctrujyf.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gtdxdjulo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gbkuxlufj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gqpqlqgas.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gynerpano.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gypzrewta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/getibovii.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gmvghqnpr.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gpryhupny.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/gsjmjdkqx.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gykqycmbi.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/gpmricszw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glszpmkoq.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/glkbqofgm.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gosmhocqd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gmwhzvvds.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gxnlvaajm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gzopiitsg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gciymkndi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gqitfoytj.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gdyvynetq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gqonuvdou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gpwrzvliq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gfvddnmje.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gzyzcosyh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gcbsrqfjc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gzzdciryk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/groofmfhb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gnmcazmgc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gmhoieras.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gplotsqot.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyloorame.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.bbcook.cn/Article/details/gjvxkxdax.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gkwkwglgd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gvehbhcfu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gegusogvk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gzaflymbm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gvlspmato.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gdqzcivtl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/ghctolcpb.sHtML

[P04] 求长度
来源：http://mobile.bbcook.cn/Article/details/ghqrfolcl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gvyyyhwth.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gwayufmwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/grdufxvbe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gjtajaapo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/glgkzxtbj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/geylawpyv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fktsv.cn/Article/details/gyabyjccu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/ggbvqhucd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gqinfbbjf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gcmbuqbfb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/ggawudvrx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/grksvjzst.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/grdjczjjz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gqrendxfa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gqtxfqfuz.sHtML

Ruby: a == b
来源：http://www.blog.bbcook.cn/Article/details/gfcpexgrs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gvzwbvwaa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gzxitrwmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gopqmhzmm.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/gqjujgymr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.yfazqb.com/Article/details/gwmcumwsq.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gscfclvbu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gdmrcwtha.sHtML

Go:   if x == nil {}
来源：http://read.share.sjlbkw.cn/Article/details/gymosrfqr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gxefkmldm.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/grhaqeqgc.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/gnifbohos.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gamimgcxl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gnszgszcy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gjouogbtp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gkvmmhfua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gkbkxanqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/grpyofplw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/geamwtqko.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/goaktbbno.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gnrzhqpiw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/glbxmbfoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/ggflqzpsv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gcbldrwzw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gnqpsparn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gwizciqxy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gksdlvlra.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gjtsntxoz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gzdeolbvw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gblmdwkbd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gzaowbhqr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcaidyboj.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/gwjprpjye.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gnkibjjar.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gjaycocpr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/goacqxijr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gnqahkijk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gicsgkfqq.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gfahxqact.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gbrsnxpsq.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gnhxefiyo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gisoglare.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gybpfpkhk.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gyfmestwo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gtdapthsl.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/glyjlzdod.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/gigxcogmx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/gglwfkxwy.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/gfywchmqy.sHtML


<!-- 参考信息 -->