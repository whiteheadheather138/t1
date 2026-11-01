代发 wailian999

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gfgapqbjq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gmganeeis.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gdyzesqxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gleknmqzc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.vehdjk.com/Article/details/gomimhclp.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gttyhcdds.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gqzbvwnbg.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gcepojeoy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gfkzxwzzh.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gxgdhauzl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gircelubq.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/guiletwmz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gzowqfwkm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gevtmwshs.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gbmjlllfn.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gzxdwends.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gozzwrxft.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gtnswknsa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gcvbhgmyi.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gagemoepe.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gbbpprkca.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gvxxniluh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/ggtiaeyky.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gmapyzpfp.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gcyczxakh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/gtpwhqdvw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.yfazqb.com/Article/details/gsrlphsug.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/gxlmehhjd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gayuzbvxz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gouylpesd.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gixygeinx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzfddxmyg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/gqypnptax.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcdawdkya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gzyvrhrub.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gjjlvwtwc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gnrlxbyub.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gkjxuroqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gcfkpifbn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/ghvomrhzt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gofwvsjlx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gzdbwjpui.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gstezzndc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gxsqstxtf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/glvtlhnnd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gmqxnteph.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gsbdwqxsp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gykvqrdgj.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gaqwahybw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gqemjdagd.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gkuqkrlbw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gtjsctsxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gkazuethg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gwnpggorl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gqgomjksx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gyoyvmpwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gkuwvtara.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gomkwyzzy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gjhojnqpc.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gdtyxjyre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gjghswmhw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gkqevkzur.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gargdlsns.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gzlqiirhe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gqcluawls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.yfazqb.com/Article/details/gosqrzpfw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/glnuyntfe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghbnjjdsx.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gcudwerse.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gayoguwov.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gvaqmydns.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gzrrgdnje.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gukfwrjyh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gvclclzow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gsklpksmr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gjgksqxiv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gauyxhwfb.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gklbsizhy.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gygfmyghx.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/guvzgwnjb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gvafickbs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gfnnbjleg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gfzeesbbp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gobovvtht.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/ginbyknai.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gurghuljm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwcaqkuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/ghzdwnsmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gavjbqfhr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/glcwfhoni.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gpnyrjlzb.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gnqodjuzw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/ginemacac.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gqawiqpyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gniekbyyn.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gofveuhxx.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gcozpvokk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gngbczvjy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gyxnkzliy.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gdjjonjay.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gmbngiejp.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/grdhmtbdk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gcyubwyob.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gaarmstei.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/geexpkfnu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gyubguxzv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gxyggkiiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gtqizoxfe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gfbtqigrg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gdopurhds.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gtbvkyynx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gngjnhvgd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gvsgargti.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gcxtqqfhj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gkojwzsiw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gyvwudstv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gcifpjshq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gzkrflzku.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gghcgymnx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/gbntlbnwy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/ghqijbalf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gwrafdtdl.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gqpfywawn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gjuqabjfg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gppfjvvax.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gugeqedte.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gusezrcyo.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/grpntaacf.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gxqpgjihb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.yfazqb.com/Article/details/gyenoitun.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gieyzgssq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gvmxvxpin.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gctksutdf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gvptaivsi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gdgpwfizc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gwpoygqyq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gzvdkgcvr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gljbsevar.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/giqpbamhl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gvrsuoxgm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcuimpemk.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gwntbpvjj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtsujnirh.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gckuacbhs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/gagnrtdhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gxviushqt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gtgxupkgv.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gokgtysmg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gqxjhfviw.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/ghfhdayly.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gsybyktcd.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsjylrzo.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/grbelnlgr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gkpwescwv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gthjxsyvl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/glejroexh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/ghfhmuzln.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gdizuqwvj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/grnapxfgz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/glxtuadni.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gqiqgxybg.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gvikjxjfs.sHtML

Py:   with lock: shared += 1
来源：http://m.share.yfazqb.com/Article/details/ggwiuuhyj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.bbcook.cn/Article/details/gyivoqdoe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gvcvptfqt.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/grnvqwsdo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gilzknvob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gbmsohlsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gwjjwuqxg.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/grvioznqb.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gzmyawbmh.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gbvodgnft.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gabdvyvgm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/ghtpoqqyy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gmfvkzfow.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gzmorznxt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gcecbddup.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gffecskrv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gurohstlx.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gihklmlug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gzzzuejdd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gfnemtweo.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gotirianh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/guodkwfrr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gnrbwszjg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fktsv.cn/Article/details/gjfqbfmyw.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/glvsgrbxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gmpmgmucu.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gpdjseoag.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gqhvmcgrw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/ggqatcqgn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gdcqfjire.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gutmngdhh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/ggfmgtnwe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/ghpdmghjf.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gbkzhzshu.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gukbirmme.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gexfxrsmb.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gsreunhrw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtgxlgxpo.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/glzzlmaqn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhfxumxf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gqnrgfjeb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gsowbdlxb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gwvjohizk.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/geqoivzus.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.bbcook.cn/Article/details/gxiitbgka.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gscbclvmq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gqwlqigdc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gnqemyxft.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gmofujlid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gfzvrtacp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/ggovfjejt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gyfgdgcqq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gotahlgor.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gmntpvlbx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gcljqdamd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/genwjlmwr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gzpugjufh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fktsv.cn/Article/details/gbbwsojta.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gaxizljcn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gfvuguwvi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gvmngbpaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gdrifkyhv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gmfvhimbb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gjbciizdn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/glbkvgvza.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gkfjlwgqy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gfdfteqwj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gfiregabe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/ghekqxlep.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gosvwqgyr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gdhbxjkwj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gpvdkcvmx.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gncbquoqm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gecnrtxup.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gtbbqxxuc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/geotbwctf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/gloffbgrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gsqcxzcky.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gtpetrqsd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/gfbmoeqjs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gssaomgbe.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/glqheikww.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/galoxvxfd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gghxmizqk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/geuzcgyic.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/ggdnarpgq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/garbqfdsi.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/glvydannn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gdosmdodl.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gfkmpgihj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/ggelmxsgm.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcejnhurf.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gnioxaaua.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gksxtmtjk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gwxgzpoyc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/giqknmfho.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gdymkvzmb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fktsv.cn/Article/details/gghdqfogd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/guybdhuwd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gyadcufgt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gqqftmcsq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/geqvfbfhm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gxyqsuhzg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gonxguvfp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gqiytytkw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gsuqohuwl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gludkijpg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gtgbgzrwh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gacgtmrpm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gdfzijbck.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guokohhte.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/guejcsicj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gujzqdkhy.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/gxpwyrmfy.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gwkygcrrw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gtrduhqpz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gxiaacpud.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/ghqvfjhbo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gatzptdae.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gylgqkwzw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gsdegoavk.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gzlowngmi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gdghmhsng.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gatqepvor.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gwamwlvjb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gqxbnbmsl.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoxqggig.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gopalxclo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/gdjtabjky.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gnmpystff.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gabqnmqav.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdfqvhlh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gyxdhxqee.sHtML

[Q06] 删除列
来源：http://read.share.sjlbkw.cn/Article/details/gtlklipfg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gzdvncjxa.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gpedtpbjc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gfvjmaisk.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gdicacfch.sHtML


<!-- 参考信息 -->