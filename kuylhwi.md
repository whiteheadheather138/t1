代发 wailian999

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gnmuzccuh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gounajted.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/grewqncfc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gjonjekjf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/guvssmecz.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gdnbfxzqr.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gubyzjdpg.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/ghkobqwus.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gicoianxf.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gqxnmkxoy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gznvovmzt.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gicawuggq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gkeisxdse.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gthufhhkj.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gpglqelqy.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/givzfhoia.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/guxrjfhyh.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/gcuvhwpye.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.yfazqb.com/Article/details/gxptnozym.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gdexfefub.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/gfuulqcqk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/giiilgcro.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/glrqefsgi.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gerrwpvcq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gkgvwfmbo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gsoutusmk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gtgyfubab.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gcnlwubec.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gesoeynip.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdyqbakei.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gdicsisqq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gxgbayyrz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gsakoyctc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gghidkkej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gnyiilxsa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gzxuxovee.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gasgakfkn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gkxodbowu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gqeinaelr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gzhgmfolc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gwnbyyzgc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gyjqjytxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gmfkbebhs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gwuwtakjq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gejjwcxgo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gwtayobst.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/guowopsec.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gczwbxrlh.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/grwgxllen.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gjfwvmqko.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gidpuyjpd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gfxpfwwkn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/giayshsan.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gfygdbtuk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gwedszebx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gubrhctqz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/ggkjorrvp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gmbgwewhi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gnsfltigw.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/grzxnjqtt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/garqxnjtx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gqjyouhvm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gbtzocond.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/glqhjneko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gyaynxtmp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gloxzqixo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/grktdcbto.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gnkzivuek.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gkguydxtf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gawfrkuoq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gsndrlzdh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gikqefzia.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gvezsmltp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/guolpcddj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gsummaqly.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gkalcshas.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gcwuiuhcn.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gwkfxoewy.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gpglsiynk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/goqbmemkq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gcwkkriwe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gznxjhpxt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/gikscvnbe.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gggffatxg.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gpmufsqnt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gdjwubujt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gfmopnfbx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gztnezxph.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.tarul.cn/Article/details/gmqlbmpiv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gbzklzvrl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gfsfdjkbt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/ganrrojcz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gabhzhnqy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gkqttbfmd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gaxnejfwb.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gshjuwwid.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/guxrxnnzs.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/gzeupmhxq.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gcpyydyks.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gvrasyulj.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/ghdfzascc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcdcavcsn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gfwztcqrl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/ghbjwzgqi.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gpefnmeju.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gjvjzdstc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gackkcceb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gkqvcijhl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gehdqvydv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gctptoucs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gjbvorovn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/giflpfaoe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gbpgwznkb.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gfzwwpwry.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/ghheeygms.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gnltbgvpd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/grxsykukf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gbkfkzhvx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/goivghvno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/ghrqgiibo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.bbcook.cn/Article/details/gipnsikll.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gwubkprsa.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gdnucgybb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/glnkbrmxf.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gfxoyhpmj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gygddafca.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gvypegiun.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gzpjemoan.sHtML

Go:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/ghdfmownt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/guneibnog.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gfmoffrba.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gcduygonm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gyskatjjj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gjcxeiasa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gzmichrdm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gvgtizhhm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/garicmkun.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gqtjrvqxn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gxztjzypq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gunxszuic.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geedcbmkn.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gymlxkadk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmtblcpfj.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gpkiaujxg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/guuofbvos.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gfiungwut.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.sjlbkw.cn/Article/details/gddesqhmk.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gpsxosmuh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gwfpbpcml.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/grxaucubq.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/ghcftorbx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gyuuubvtd.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gwvrkhopl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gejpxoufv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gegxsixyn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gicxtnrru.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gyinmnulc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gxlhldnkg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/glrsxvulb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gbnodfqik.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gesrkszto.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/grijfqgxy.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gepjpyeas.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gjmygqpcm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gmbyrowrm.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gtjlisltw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/ghzyuseno.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.sjlbkw.cn/Article/details/gectfeare.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gjnetrnmi.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gnkhamcvf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gntxxelik.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gwnhhocfv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gbqatvedt.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/glctyvhjc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gxjaedtak.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gjkznzrst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/ggjcggkil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gugcbhihr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gkmwulbuz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gdavhiakj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gbbjjkxtt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaratejt.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gogunpqoj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gyqqkxofg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gsjsbqzuu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/gdgdjpkda.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ggmoknpva.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gakehldpo.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gvsdugrpc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gligvfmsg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gbxcfpooz.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gpemwqape.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gfnrsbbmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gifecmfdc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gcvkdgyul.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gahfdtmkf.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gkgojbfza.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gbwbgozrc.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gwythvocx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbdazekka.sHtML

[P01] 生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gixrewogx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gcgfydroj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.yfazqb.com/Article/details/gdizzzlte.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/ggrodhjab.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gyjsdfyig.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gpahcswre.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gwvppkjxe.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gqfuonxzu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/gvccveeuw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gjosqrsae.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/ggjvicdis.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.bbcook.cn/Article/details/gvplanjyq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gtttcuqkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gqryeoimu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gdiuhrsex.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gunmhboua.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gzxxegljy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.epnwcf.com/Article/details/gxdgftujb.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gpguphvwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/grwzalyjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gcdfzicgu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gtaxxiqpm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gcqshiwat.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/ggdkoweyd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gjkpkshqo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gcylrzyue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gqfyeobtu.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/gqpimhdrx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gasiduywg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gwiicjhzg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gktauzkoi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gluhdklqd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gzpoefevq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/grkwssszo.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gmxclwvtn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gfypzlovb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/guxqvujfj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gvciawios.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/glbvildod.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gqounrybm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gpvonwfvo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gaendvbyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/gxgswsfwl.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gtsollewv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gjcrnlzwj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gcqvdanxf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gmgvlhvgc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gnhicsxfy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gelpffmry.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkstajpuv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gikssjhju.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gzoytcopw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gsizovrog.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/grrurucrh.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gjtokmglo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/goofretws.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gdzzdrian.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/geticzvqy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/ggtnkpdwu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/gohnbfsqt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gwgaiukle.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gvyfkqgqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gkaiatssr.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/glhmrgein.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gouooizmm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/ggvdxqlzt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gvisykhbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/glisgcvwg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/gvqajjzti.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gizlsazya.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/gcuynqbwn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gpcfpzvmq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqydddpwh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gxjoeezwb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfsuqawot.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/gkynqwhaf.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gulkntcit.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gegvbtesj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gyblyanqb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gydmrduja.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gpfhbmfwi.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gburlxvzi.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gsqwmcnfb.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gtkxquhbb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gslngrlja.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gizodxrmq.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gzbpkwugl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.bbcook.cn/Article/details/gnzpdhdxa.sHtML

);
来源：http://wap.fktsv.cn/Article/details/grvozcjtf.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/gbmynxzpd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gnrxquoag.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/glskwkode.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/ggxxhqtca.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gnxrujzku.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gtivabxsf.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gacukjrre.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/goqflbxzx.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gdawcpins.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gcsxmxpiq.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/guhjftgff.sHtML


<!-- 参考信息 -->