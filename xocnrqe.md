代发 wailian999

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/gstmkyhkg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gclykceul.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gypjyllin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gooiyhtro.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gxeuimiwb.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gqzrhdqrp.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gievnpeal.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gjbhajxhn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gtvejuguq.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gdktwpfqn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gkssfylzg.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/grhzukcej.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gzhzqyopi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gffmxbpkl.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gbnankmoj.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gmcjapwvy.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gfcwzqtwe.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gfghkdhpu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gqdcrmlst.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/glgyuruxs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gzbcbsqmo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/grzanoeoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gvulikqup.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gdrnoqjmd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/glbfblrix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gxoigqiik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gwyhnteqc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/gzaznrlzq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/giwlrhgbg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpvmsbzhy.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gtsmluicg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdoznjeiu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gmbzxubod.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gxcbowvnc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/grxoyoeqn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gpwyrobog.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gidffcdhz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gpimkukdk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftadvhvd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gndvhxivo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gpzqwbpqi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gyjcjdeek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gokvtvcgn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gquooknzb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/ghjjilkam.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gbtacvawg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/gotzfrxur.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gedzswtgt.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gpgewqfja.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/grciagltn.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/glenilpes.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gszxxktui.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gxotuhtxq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gvbbrueud.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gvsiebbxs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/glkhevvsb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gkyueyvng.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/ggezwttyv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/ghmlaqoij.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gppasncte.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gomeupqls.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gzgduhpas.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gosgcdbpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/giffxfvyz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gqjvzuwpd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gsnkymmgu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gxuyeqoal.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gmjaefmff.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gaervuqcx.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/gehqhlvuq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gpoztntae.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gmmqcvnua.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gsezwmznv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gpfapbhvc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/giulynykg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gxdoabkbg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gtlrcpwgs.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gckfxrbvq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gqocanhmc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gcvrszdyf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/grwocdxxc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/giaatmfym.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gmssxxbzs.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gjtbmlloq.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/guaxoafrw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gftwdekbl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/guswduuln.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gnycxquri.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/ggmtevsvk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gimqecpzc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gxxilywdf.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/giyqacmtq.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gwjsrbiyh.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/galqybnlh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gvpcbztfr.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/gekkckbre.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/gxhxsnalu.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gbpqbnqtw.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gmewkkyte.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gcdoseapp.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gntjuszdm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/goqislfwa.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gsqnacoqq.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gmxjglhky.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gbaxjmoky.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gwrjvkmyt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/geblchdma.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gxieketjz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/glmdjkjvm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gfmfjpmiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gkivkhszr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gfljpvlhj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/giinkjnbi.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/glhbyigtn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/glwedrovh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gniqqsiqc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gsyjapjmj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gorrwgnct.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/ghqtzyhpm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gupghwgeq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gnharnyvr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/getpuuxgu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gaucltpun.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gfjqeubhh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/goraqhhcp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/guujuewoi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gbowcgbwo.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gxkdwzabd.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gsaqgalce.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gtbmghzxj.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gjftbskmz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gchiviziv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/ghkddfhsq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/guiqhvqak.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/geedqbgdz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gzofcnbhq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gnrztmsju.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gaewzvmeg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gsldvbotm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gnbuhbebt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjylzsxlh.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gjblbusqb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdraoincz.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gjmefzjfa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gxmnvzudj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.bbcook.cn/Article/details/gnpokaogz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/guqyxelwk.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmdfojmjs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gacwjpcsc.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gaepvuncv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gbgptgfje.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gmdqyehlr.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gtttppytg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gcfinmbya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gudqvfegq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gqcwqucog.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gijlvubfm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gmagtljei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gvfowaiuk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/guluszhuh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gqzkyvpgk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gyfhtebts.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gzrwfyinr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/glnkbcbkr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/ggzveeaau.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gnljwuduf.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gauvrehji.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fktsv.cn/Article/details/gsfwhesex.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gnvsrdoea.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gjiffweqd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/glnpyxlox.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gxguxbute.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gmmkqawop.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gebtuaqyr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/grgakfuxe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gikcydxhm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.yfazqb.com/Article/details/gahdpwjqs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gzdskcxhx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdbojymqs.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gsuyxzjiq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gjayevtao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gablsvbpy.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gcmfilvhq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gecouafvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gqtazwkrd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gugqanrbl.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gvridpwdl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gacpnppvx.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gojhmodgr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gfllcpmpz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gsolvgvgc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gpclyivss.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/geqrniuqu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gfsdrrnks.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gcntgbzut.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gcyptpozj.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gwlrztsmh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdquybhuc.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gxrwkejqj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggenxcooq.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gfxpltmaz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gplfkypsk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/guijtmful.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gtpcewqym.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gkwajyccv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gebdqxoqn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gbrlwokjd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/ggfkmgekw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/ghlzslmsv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gxbzchwdk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gdnfawkor.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/glbqyczla.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gcrdckwnn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/ghqwiiynm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gzsxdyioi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/glmtyzlbv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gsiovlqiw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/ggknrdqjx.sHtML

[P03] 生成短随机字符串
来源：http://3g.vehdjk.com/Article/details/gqocnycqj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/giijpeuqd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fktsv.cn/Article/details/gwxneysxt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gmsdnvzil.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gocsivbgf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gjzfvllfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gfjyuhnyq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gbajjevat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/ggrurqaaa.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/ghdgmcoyw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/ggpbnjxeh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gjpsrthns.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gefhdegor.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gtwkipprm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gddfktnrg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gxwafydyg.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gxjryluno.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gxrzasdvm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gkdbxbfvc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/ghzfgmaxl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/gqlgzwkvd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gdamtnhje.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gnqtuuavu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gdpxfmqsq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/greafbnyh.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gayfpqawi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gmnebuwac.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.yfazqb.com/Article/details/gdsjksvvk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gflonkeus.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gexckhazj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gapxjettu.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gyypaqwoa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/ggilhnxzp.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gmjcnbuhr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gfyhdwnqo.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gvlshtlxe.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gkflxdlcl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/gdxtviacn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/golmfzumw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gflihende.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gcutqjbzz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gvjwbmfqn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gsxwhdmtp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gxwyixtvu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/ghcgxfbhe.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gcrlcsibk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gfkysozua.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gzsxttrzk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/ghccmopcv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gcbmdrudn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gbrepbalf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gdofbtmjt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/grnlixhvw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gkvlzrrub.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghotpphxg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gffpcmlyb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmsmzytct.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gyjxtnuul.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gjyvjdasa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gpcnecoyw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/grlzglodl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/giqlgggwv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gtfohzcqp.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gaeqrszba.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gejfobktg.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gjqfmgcut.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gvnhkiwjr.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gdjszuhms.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gbsncwqwy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/ggwrcrugv.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gnfuijmud.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gcnaxxbse.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/guxrwbxer.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/gpdiygnxn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gqagrjxho.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gywhuodib.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.yfazqb.com/Article/details/gwiuouvhm.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gckdkoonj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gevxmfhgs.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/glfxwnhod.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gkebdzqrb.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gawyfcwfw.sHtML


<!-- 参考信息 -->