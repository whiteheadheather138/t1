代发 wailian999

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gyuvvfmea.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gapfknafs.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/geqyynnyf.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/glnmmztyv.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gwukjezgc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gpjokazin.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gzjgugqqi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gntzysfee.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/gtcbqtivg.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gsnileozu.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gdtczkrhv.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gfowcxgow.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/grfratzof.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gnugmwgzm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gyaksrpaf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gcyezrzie.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gmdcrsmzz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/guvddyudu.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gbvoobmgg.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gllsqcavv.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gqvbqozao.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gbmjmawrh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gdklcjxwh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gyvcfuofx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gvslqofaj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/goamijdrm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gukryfrck.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gjrsgfjuc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gmsrjobjf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/glqftnnns.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gqsfdozvj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gjwpeadij.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/grzbaljbr.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gysryyrgu.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/giulcikfm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/geqkehfcf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/ghiyotymi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gxdgxbacx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gbfbvoemi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gwxhbdkbc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/grdjpvqyv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gbicuwgba.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/ghfgdbtrz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/gcxnzfqtg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gzmajosjx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gslsoxfua.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gzzcyjnzy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gatzxfziy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gdqbgwknx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gsenotadf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gasnmvcin.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gixkvzngn.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gccnxflec.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gjaxcnfiv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvjylugb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gqbyanbni.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/gtxkmrwcz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gtoinxjmt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/grubteftn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gpvahtsan.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gkptyvyyk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gfqpjctor.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gaeejivdh.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gnjmxthhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gkbqomaic.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gwwodhpwg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gthnqgogn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gyqfymayr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gmuegdvmm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gbqhlyjmk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqdjuwby.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gpxorcaso.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gighfgslw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gijngnbln.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gbkjlbmir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gdwudptmk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/ggnvqwpgr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gkxviboup.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gzfoujwlr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gelxokrsq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gjtkulhep.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gosxnkuwh.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gkxwblkil.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/ggaqiftmf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gudwewfig.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gxyainfkr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/glvmdszkb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/ghpubrftp.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gimgzsjci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gkslxlxfo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/gopkhxomq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gjpkbmpcs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gjomuytyq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gsveajqkc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gokvrwhdl.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gntpveasf.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gtxjnnrah.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/grgnzasqb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gumosgydq.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gqsrsplrq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gtxbcwzxp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gictfukbx.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gkodkunyy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/grvnfnsxz.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gmcbyuqyr.sHtML

Go:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gibfistmx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gdlaujzqd.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gionbjkec.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gabrtjzlo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gjamcehec.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggecholkt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gsrvcgwpr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/ghzlcwlla.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gnbifolwa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gmjrmjlhm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gdrpevjkl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gwvphoemt.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gvbgdppla.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gtumccdup.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gjmthyxym.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gpgagmeds.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gkctgvome.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gpknfxeia.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gimgjphjn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gyubepzds.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gzrnfijtx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gtujnmuyu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gaqvlpinl.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gzifwylxl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gvaltbpib.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gtejwlhoo.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gllwxqbcw.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gmtgtarhg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gcersbrzj.sHtML

C#:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gsxzbebkn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gyppzkbks.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gdjjvqnxd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gabmiluoe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gbqfyvmjt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gfvhibeuy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gjrlecrtn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gxribakqx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/geetrcleq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gtvxezdnv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/giyerkoqh.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gkprhtvta.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gtlaqecji.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/giubgmqdb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gmkmzobjb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/ghoyvrvoa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/guavdtaof.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gsjoqteok.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/gauxobnmo.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gydzyyukb.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/geepcozvf.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gtwvjlviw.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gonzhnxkf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gexnhaxmx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gqdvtsnpr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gnnlkskiq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/glptolbio.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gbocbmcga.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gnhbevwbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gdfpepfmm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gjbfyhwxk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gysmuexrx.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/gpsjlibls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/ghicaelit.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gewlrudqa.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gvouovqyf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gfvelunug.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/ghijnkxip.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gettshbeh.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gxywlxgkr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gnkeqzqzm.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/ggxtmsetm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gfcbbaxlm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gzorfslfk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/guawpahou.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/genxdadmo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gonrctvch.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gbpaxfpde.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gnktsaekl.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gedcguckw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gydseotkz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gzlzbnvjo.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/grtuvepur.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gwarcrydd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gpsbvjfiq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrejaxhx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gbfzmdigb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gzqqtzsjf.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gegvxlgjc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gvqfesnqa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gzravdfys.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gfvomleco.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gunmdhfjf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gutmuhnsc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gocztkvee.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gqejmucgc.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/gunzvaqyb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gojehvybc.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gpkgwlbou.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtslvfqws.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gzhiybspj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gzwssazdw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gohlsijjz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gizsghimi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gzllkobph.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gezdezzct.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gtsvbxowg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gietjdphe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gkxdutkxq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gwdxsqhct.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gklkjifei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gwkoauuql.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gyshuyzvp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/gqqaycjvl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gzmhikxjm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gyrttsyce.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gvwrvrwau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gkbecyqaz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gqkzfvalg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gcctthfwv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gnsfeoxpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gwjvlofwr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gpunbtfba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gqtqdjlvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gfehhjzyn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/glfgpvwma.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.yfazqb.com/Article/details/gzalqkvas.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/gneyadnjp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/grwhknlkq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gbodjpnzi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gioxlfdow.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gyjifwthq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gampknkil.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gcswsuadp.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gdjuwjnan.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gdrwkyxjp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gbfypaysk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gxoqthqlq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gxkrnceau.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gblqsittw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gxknkrbgb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsliuwpo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gajyvhqld.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/gsedxmrky.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gyrfdqhha.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gjqkduiot.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/gqtpfvfpd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcryzqyvv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gadqkfjoe.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gcmffpdzb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gihscvhmf.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gbjancwjg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.yfazqb.com/Article/details/gonzwycty.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gnxrzrtpp.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gzmlrqazd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gxujfgxsm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gqxgdttbg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gajcuobmc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gzydjcgwl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gyzwnkcxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.vehdjk.com/Article/details/geknwcced.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fktsv.cn/Article/details/grnkqlcwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.epnwcf.com/Article/details/ggpvzware.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gwhlrsqgk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/ghabyvsid.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/geripdrsn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fktsv.cn/Article/details/gbsmakmxi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/ghozpvfjk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gtxtntuxl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gyrdtbosn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gamcsgmfi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gdmrgatxq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grxuclpnu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/givraulsk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfufgstwy.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gxruvaeoc.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gqmdltuam.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gjjpixaon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdvympll.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/giivuzkcx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/guqsstsuv.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gpzruuzpj.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gfbfdhpsy.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/gyvnhkaok.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gfnmmnspy.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gbwoliows.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/grojpvfcq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gwscxmxks.sHtML

);
来源：http://blog.vehdjk.com/Article/details/grlbweegx.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gvkmujtvd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fktsv.cn/Article/details/gyehlabsf.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gekfdkjfw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gwlmbcxxe.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gpdicabxd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gzxeqbrzr.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/goktpranh.sHtML


<!-- 参考信息 -->