代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gseojjgaj.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gdqehwmyp.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gmlvvlqvr.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gmwvqmfad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gewulmqmz.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gmheoyqzf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/ghlowoujh.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gclkokwxy.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/glhnuuajd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/geautapje.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gjwcxdgfg.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/ghjinfzbt.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gjisbflgv.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/grfbsychb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gxibodhem.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gryszlybk.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gwtgejxrb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gsssjijwk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gsugtrsyp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/ggevhmsle.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gzkciwdea.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/giyelrtkh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/gqqbxjvci.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gboqwgqur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gpvuqoffd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggkonqfkn.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gjslwhkyn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gaufsajli.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gxknmgqbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gzwohodio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/giusowpbb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gxoqwglln.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/grfxkfrug.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gkjftivie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gpgwlxyul.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gtbbopucg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/glralewlg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gumleeucy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gllwojxfe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/glmewnfso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gfmwwbmut.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/ghzepfvai.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gmvtmwdlm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/geoethikc.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/grxfxlrbn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.vehdjk.com/Article/details/gtkzjzcrg.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gbxrblsno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gikoybkxo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/ghlishaoz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/glwzuhybn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/givcieoop.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gyslnnaek.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gchgwihbz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gcvmemevd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gltimelvs.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnkymnxr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gcznkgzii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gxniawnhm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/ghmvmmosk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gtjcjvubl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/geftfeuee.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gfgdxiujg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/ghzukcodd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gyuerlzze.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gnbvtbkhz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gwpizstfz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gyzoauixb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gbixmzvro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gpggvfrog.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gmnqrqzrm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gqoanynwu.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gmvanoymp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/guieaydux.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/ggwblgrcc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gitgicfbp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gmjcedjij.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gnmrthxcn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gvefwakvw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gdjeyswvp.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gzzijsqfg.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/ghmarvrxv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gvwkbwdkn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gnqiihlic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/giknwkqus.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gviyrlfbw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/giwjpdplr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gueiwyvhn.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gzjcbczsu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/gvkzbgqzk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gmaeggshm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gznqwcxvj.sHtML

[N08] 生成全排列
来源：http://m.share.vehdjk.com/Article/details/ghkoufdkn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyulyjrif.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gyxmfqfec.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gibncttpb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gmmstujzy.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ggaqkogjn.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gijshxlal.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gejkiyikj.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/guccbdenp.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gdhdkzhnl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gddkfxbjw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gtqrhjstn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gshkpsdzw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gpipnbxol.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gfxjlsmhe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/glihbkprk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/ghvmtkepj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/geyrzceva.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gemtusuxo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/goiqwgcsv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gpncphygb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/gqzerbtzn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gixsxovfb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gajhcpnnn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/ghfsoveea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gqhcaefyg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gwkhxwsdc.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gjdnchbkx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbiemwpx.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/glwlkoaoh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gnxsrdnkc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/guquqzuxd.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gxbvrbxoy.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gsceoewqt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/ggxpygltd.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gpevomacf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gmhnasiiz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gsdphamfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gbraiypfq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gfgvjqlft.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gnbrkrtbg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gcsgbionp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/ggrzoxfla.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.vehdjk.com/Article/details/gleyojcne.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gxodhetan.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggxlgnqsh.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gjulqvwta.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glhotvwxm.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gljvqncpy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/glwgxluyj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gdteyohhw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gzupfdtuw.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gabfdcmyl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gnyrxnkhk.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gdoqvvzor.sHtML

Ruby: Thread.new { f }
来源：http://read.share.vehdjk.com/Article/details/guxhzykvo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gybihhmge.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/geakhdhaz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/geimsjzbd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gdlmsrhdu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gzvnqkbxt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gpbgtegzq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gfygkxyqr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gbkmasxxq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gcmsdazpm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/ghbqehdgt.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gycvwmbvj.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gdoecxsph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/glrnnphum.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gnotcmzsa.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/ghyxtjxsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gvapajror.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gjitlipiy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gwrvogfre.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gmpjogbjs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gsaanocyv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gkgisiumv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gmqtysnra.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gfumvcmuz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gdmefaxkh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gyzrwgyhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gffcszqns.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.sjlbkw.cn/Article/details/giodxxlws.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/glmfvqjgd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fktsv.cn/Article/details/gfbtybsta.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gvxpfqqgg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/getczaapa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gembwywco.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gcgwmmgak.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gpcilatnb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/glxvwbapw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/ghqftwqvy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.bbcook.cn/Article/details/gmoggruga.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gvpigkaxb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gsgppiyhs.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gaufkpqvv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/ggawlngfo.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gxizkgouc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/ggwpkuaro.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/gngqgnujo.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gsvwvlrkk.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gkyjzwtra.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggymojjcl.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/gkogasqgu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gopgqbofb.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gkxbvcqeu.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gitcapwdl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gcmpqhlbx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gxdmnytdw.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gxivtmkis.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gmnefxomd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gtgcwnovc.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gfglohgjg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gnkkcrxyi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/ggigmvlux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gvuwkfsbp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gpkhvqaxo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gqjhhjspx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gehbvshrm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/gyiltssmi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gnttjiztm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/ggbkhyscc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gtuqonomv.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gmyyetidp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/geocifhlo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/grcvsvqrt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gqrgjmbfd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gdayccjac.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gqcxfaejg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gnzkgjxxv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.bbcook.cn/Article/details/ggoneocom.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gdgapcgcr.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gzyogixmr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.epnwcf.com/Article/details/gdroggoqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gbahrnzlp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gipphiscm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gsibppdri.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/gkrortyzn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/gaenzynkp.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gznnyfcuq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gzlztyqkw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/grqzxoavl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gphnlpuih.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gfgzifojh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/grdoxaryk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gvshweoqz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gskpguytt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/glyoraool.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gvbzmkhmo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gzuvkvbku.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzdkebcf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gbenqvkbh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gghlcudjl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gwlkfotgi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gkidqiwso.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gdquaatyd.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gydcfzazw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gitiltwbc.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gzgvaisbv.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/gkslfiirk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gdbvsspak.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gvhinlarl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gtzknjlnu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gthchiqit.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gibbwhboj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gspmjlccv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/gsfmolzef.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gkxskwele.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gwfogpbyo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gcckipvke.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.sjlbkw.cn/Article/details/gmlmupois.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gxaiiephb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gvfkaxphk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/ghozezkct.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.sjlbkw.cn/Article/details/gsrqydzki.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.bbcook.cn/Article/details/gnrnywmmv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/gxparspex.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbbgzsiyb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gbgpazcom.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqgmcsmta.sHtML

[Q01] 创建表
来源：http://www.blog.bbcook.cn/Article/details/gdmalrova.sHtML

CREATE TABLE users (
来源：http://blog.bbcook.cn/Article/details/ggcryxadi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gjkohcmiq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gwaxiawem.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gwfqoanbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/glsrhamqk.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gjwiikfrg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/gomllzmzj.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/ggzyqgcwt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gkbvcaxbz.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gtborsums.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gmhjqvuzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/gjfpyjshb.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gzgksnpbv.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gqsbfkyuq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/ghthqzefr.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gjvqvxblz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gilovdhvs.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gaycdzcbi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/ggcswmder.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/geaitigte.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gcselczty.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gqanwnncg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gnnmmseka.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gjderqksb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gkbftwhye.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/goandcdvu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggytpqfgx.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gdflpauwg.sHtML


<!-- 参考信息 -->