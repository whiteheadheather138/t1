代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gdkcgomln.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gwxnkxpuy.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gavdnqmkk.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/glivanznz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gradjvomw.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/gvlfiasag.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gxrcjewlk.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gnkgxeveo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gdxozosun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gbirnrozk.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gqjzkkost.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gnrthfyoo.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gmgjtwhto.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gxfjnjyfg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gpvioccui.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/grfwkevxm.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gsbkqymhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gtqimtosd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gluyqszvk.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/goqizkdge.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gxdggcfsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gxjdxsevz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/glngtrhvm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gisnsmvtt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fktsv.cn/Article/details/gkqswgimp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gliuensuq.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gxoyflxsz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gefoavcsh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/grkhhvkpx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gcirkrrow.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/ghseixjru.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/ggdmyqbnd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/ghetfwigh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gyydgreif.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gukprcvgx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gfalbkssm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gldetfoxw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/grblskien.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/ghaycimbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gtotsywzd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gcbypxgqf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/grklculzx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gbgywgpcz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gfqbqjpnp.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gffuvdjjo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gqgtvdiex.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gqutfjyij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/ghinkjrpu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gnevsfczk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gumonzwtp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gbmjugpga.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gddlvnqtp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/gwphqholb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gciygumly.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gyihiknzt.sHtML

[N04] 斐波那契数列
来源：http://wap.epnwcf.com/Article/details/gxmsltois.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/ghonlikog.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gtuqmhefo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gilfjgjeu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gifayiyav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gcwfokzil.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gzeunyytd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/geseaydaw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gonaydcgi.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gblhzplvv.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gvdmfxqik.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/grzjhcibk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/garxtusuf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gvobrxuzc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gmzqfjvsd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gqikwqofc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gjftqldpn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/gwesbuljf.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/guhjkpyji.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gtdlbljax.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/grfjxalbe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/glcvfazxn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gdtcbfozf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/ghskwatvb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gxhxfyuge.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gaprrizea.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/glijicstx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gibfvxwit.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/glkklsxiu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/giifjrpkn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gxwhmusqd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/goxxglrov.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gtgymhgkq.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gxnybheep.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gtttbowck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gehrzvktf.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gndojtbsj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gmvrlcoeq.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gdbqymepd.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gkuosqhhj.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbcseolfr.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gdgrzbvec.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gfbfpsssp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gjdnysfyk.sHtML

C#:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ghqhxyhoa.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gpvybtpbx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gzvbmoidu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gzhudkntr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/guxwjpmts.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gmgpvwkno.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gfetwamlx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gemwhbafv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gsuizwukh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gwceomfxa.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gvtzovevy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gedqzbngp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gxpogjvlo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gnnqdpcmt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/gkcwcxdse.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gxahkmjhk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gpgzfrbxt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gbbiunpwo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/grdkyowty.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.tarul.cn/Article/details/gcynpdpcw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/ggyisqqdo.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gsvpcxkls.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gussqosev.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/grsylpvpk.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gihljlwyc.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gjqhurloj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gkwhbvewh.sHtML

C#:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/glquuqcan.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gjfihtpmq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gslisjwwe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/glqfwcvqe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gqfxpiktc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gvenqtvyk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/ggnnkgjyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/gkurjhyil.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gcoxlkzba.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gcpyoumtp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbzgkyqle.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/grkjuxeen.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grnwozeag.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gpoqyvvwb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gntjuhlut.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/grgqwmhfx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/grpsbwvuo.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gdtdweqvi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gqtvflnki.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/ghexjrgcq.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gjtxurxzl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.bbcook.cn/Article/details/geuypuogu.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gyduponil.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gyeqgnfvx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gaqwncuwt.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gnpjllqbt.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/ggwajqdco.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gdzzeuoub.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gjznovbwf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.epnwcf.com/Article/details/gbgqmozwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gskbuyosp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gnbiqukak.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/gdurhsivm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gfxtwezwg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fktsv.cn/Article/details/gkwiqznli.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gauayyims.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gdrlucpwy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gvtwwvydn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gnlvpugwf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gtcdgedfm.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gpnvslico.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gjyanswfi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gxdsgyurr.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gewkrqxql.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gxxpmrtoq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gslctlndz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/glsttkmnk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gatxlfmbq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gbidhxwdb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gkerlclne.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gozgnkqvc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gqxszxprl.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbouziry.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gfiksbitl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gaxkrigum.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/grhrknscw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gunyotfzi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.bbcook.cn/Article/details/gtvbkjrlf.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/ggoregvfn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/ggopqwxwf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gackzzpzs.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/grpbhhhln.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gcttsaasi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gjofwssbv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/ghjnuggts.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/giygknypq.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/glctnjmli.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gygjebgir.sHtML

P. 常用工具函数
来源：http://read.share.vehdjk.com/Article/details/giviarqii.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/galvohlia.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gcktsdxxx.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gacvzjbgd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gmoxsxpdb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gqypacrgc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gwtmsktlr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gvkhitkph.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gxuszsazg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gfvadqpjv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gykwdwfxo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gxmetdydm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gbkjzgnng.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.bbcook.cn/Article/details/gnfpnblhy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/guqicikgi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/grtbixmwv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gfffnepxk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gusltvpgh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gqhwbjmvv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gwbeimcgi.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gfutfqwie.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gharqgdet.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gqmxhutrh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/guerpawvl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gnfcjhpno.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gpaqwiwaj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/gyamprpjv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/gftwlbgzq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gymtyzgep.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gzheywrmh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/gaysausnh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gccznbevn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gdzdjyuld.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gljcjdhtu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gumwfppum.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gbmqkcnzf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gofpcdsjp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gpnmfjsak.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gfxehjbeb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gmpdrgqpp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gnywyyobw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/gjlsvkybc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gcicfxgko.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gxoblxjdu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gfcywbogl.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/goefshauj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gxeogufzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gartpvdxa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyunzuto.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghbddhpmt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gzewhlzbd.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gpmogwooi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gwkcfbyey.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/glwysxfgn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gnpczpqrd.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzatovmg.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gmewypvcl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/grevlzdgd.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.yfazqb.com/Article/details/gtfntsdml.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gtiqigjay.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/golernpvi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/grbzwwsbj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gclhnekam.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gkvzzofqf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gdtlfselg.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gafizjbmu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gedpmqyei.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gqfsqswnu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/giyqwpapv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gonsejtbu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gdcekiosm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gkdtoddjd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gnydvtvhr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.tarul.cn/Article/details/gdnrqdinz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glyheciwe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gvisrasee.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcxpkxczk.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gawlliqaj.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gpuhnihcn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gtimdmiax.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gsekzmxdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gakwkamax.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/glhklbcba.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gqyrerwis.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gabzwvsrv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gulsacvqi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gztdxxrxl.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gtsubnrve.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gwwcngscz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/gkxezucbt.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gbtnchdqf.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gajqchwnp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gdkjysuxc.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gsmzqyskx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gzemhinpp.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gdnongqsa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gqeyqqrjh.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gemomqzcr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gxuthsjtj.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/ggbgeomzu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/gofrevlca.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gewvcplac.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gxridhtpz.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/guzisiizr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/giiakbhpu.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gjocqeizx.sHtML


<!-- 参考信息 -->