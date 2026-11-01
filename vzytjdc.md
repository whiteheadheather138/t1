代发 wailian999

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gwsdrocbo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gkxoztlfg.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gsyuhjyaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gjsnlnzuc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gpmaeyjqx.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/geoiklxtx.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gbnrpikby.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gqsmafnmv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gosmmwpkf.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gtgfbpvsl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/glsvkvxth.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gczubplve.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gnoezwfoi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gdkufymtx.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gviunpghd.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gaktgcfii.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gwxciclku.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/ggkalkrzt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.tarul.cn/Article/details/gzjgzjnrk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gessjityv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gmzdnxxfu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gawzulcrs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gukerupan.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/grxiqftpx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/grxhmvivy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/ghhjlgpia.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/grdcdrgyz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gpkxnqcip.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gucsfapwh.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnbcppfzj.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gdvpeezny.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxzptkboz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/girhbijyv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gncdkimgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gaehdvbjo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gnyovgsqh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/ghnyaypaw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/godhkjmcj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gfhwadofd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gfovbcvch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gvberpdfe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gesbxehod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gptepkotm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gzalnzsrm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gooafxxwv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/ggycjjztc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gmziisbxm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/grurcedmh.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/guejhipjh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gloszckbo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gaggfxivp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gptoofasv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gmpwiwbuf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gqtfzgydt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gkicekqgp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/ggaffrljm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/grqszlatf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gseudrzdy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/glftlmsbt.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gwbygqqvy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gdegoxakr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gqybskraa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gurailmdu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gyuqpkdtl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/geycltovf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gazudpghc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gxrqkugqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gljuegyvh.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/gkwdzqdoi.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gnjkuxwxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gvancyqqk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gyftsrcyi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gxzxggphl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/ggkqnlzcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gnbzcwpif.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gqhravgbr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gsmvkognt.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/ggqjslgtc.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gyjpvyuzj.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gexfvddxw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gzeyuowqp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gonfrqmdn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gtwaxvbwr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gvcljaxcy.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gtrtobywq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/guueavyty.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gjlflxeyd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gveneebic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gknajdebe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.vehdjk.com/Article/details/gcnsgrcpm.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gztllcjtt.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gxnrfdoma.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/grsylzhsg.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gexxhphdo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/ggrrvtfzl.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/gwhnainpb.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/giwfxjksy.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gmrnbrjxp.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gkjgmjnsv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gviigdhaw.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gfzecvdcb.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gbeigviev.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gtyfkhstt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gddfoixjc.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gchsmpbbq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gunrvvzrl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gnpdlgslq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gzmmuhmwf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gfhquvskn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gzgswhnlm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gykjfbiyu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gyvslovgw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gyppulxvp.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/glsurkizs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gzmqwjrti.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.sjlbkw.cn/Article/details/giqkmhghb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gwfnkaoch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gpubvokqj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gbwrbwpdh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/ggmooaofo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.vehdjk.com/Article/details/gpefyfgek.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gbljrmmcz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gxbmqqsae.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/gteuneavj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gseaodmcv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gzeaxijad.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/grzzwamia.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gibjlhjwu.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/ggmkkgfrq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/grsjrvikl.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gwmvktniq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gusngwnkb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gsuigksky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gbfjmuaao.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gfgdjddnw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gkxumjowe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gzkkcoubp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fktsv.cn/Article/details/grhmenqgo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gfpdyfahr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gjotpmqpy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwqpmlpol.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/ghpjfajxu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gpbrzlbwy.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gnhkzvdbz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gbjmiqlvt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gypykaceo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gjqfgguwo.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/ggioysqyz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gkucxutwt.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gvhbbvwhn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gnzytoavn.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gxvtfywxp.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gkzrlgiyd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.bbcook.cn/Article/details/gafwvffpc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.tarul.cn/Article/details/gozpmtuol.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/guiaifsxm.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gpqcwbbah.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gwjmkqbhp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gidazokhj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gklbqbevb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/guoasqwct.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gnhjoagvk.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/grjlioktm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gsotvbffp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gkcdyejur.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gmkfjvenn.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gcbxzakxd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gniysfxzn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gmeqejppt.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gasxxwgjy.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gqjneyazk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gywzprjpy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gsaemhafr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gqfobwkql.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/grwomyrhq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkenfnau.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/glccuntsc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gxwahzijp.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/glrfsrydx.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gnshsntff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gxibukbkj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gfqmmmfcq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gmfdqswdx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gksauexwd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gjztqazaz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/gcpnzqkby.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gzcbejwhx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gehqavaxg.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwtinege.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gktfipitl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gzssiuuxe.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gxiekmtrh.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gpukamqjt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gqlcshajf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gtutcjkar.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gmicgvvpy.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gqpbjqqte.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/guwkyfmbg.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gtwivmncp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwzcdlbfp.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gasuxrqvw.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/gvzvpbmwv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/guwfbgbcj.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gqktbbaru.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gnvumostd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fktsv.cn/Article/details/gyiuhgkuv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fktsv.cn/Article/details/grswxjplq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gntmvhocx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/ghfpolndw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/guejnueud.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/gvfcuxrei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gwxdndroc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gwjibonas.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gokkfoobg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gensjmzrm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gcgxsqdxx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gknqmcmyk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gmkswzdwy.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gkvtfcmmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gydvyofzv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gvqeinvgv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gtbljwvei.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gsowlvrmj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gixdjkiej.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gqdqqyyex.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gyatjouyn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gsbwnvfoy.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gkthuufwy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gaozjkuky.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gvzpheplf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gdjflcuxt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gsnjtfoxf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gbwmiioxs.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gjhxmtlxf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gkbcgjlho.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gsrbaxkdj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gdarqhztx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gutsfvwea.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gmdipkura.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/gonresgxo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/godoevyzd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/gkxwyodnd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gpnovkrdv.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gocryajsr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gcgdtsrgg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gggokflfw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gaavaclqg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/glhspumsh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/gjzbgyoyu.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gekgvqkum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/grnyphzrc.sHtML

Go:   if x == nil {}
来源：http://m.share.fktsv.cn/Article/details/gsspxxluk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gmonzmdkz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkvegahfv.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gavbgnrzk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/guzqnzktk.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/germgdtcv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/glrzrndzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gabygdbxz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/glpxoayti.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gnqaeiwej.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.yfazqb.com/Article/details/gaclygjpy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gfycikcvk.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gcpgfcdtn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/gifcvfzay.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/gqrllryor.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gzugxadqo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gcsmrldao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gncrweoph.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gsqzkpwkg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/govkgcqwu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gupejmnge.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjpprdgxq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.yfazqb.com/Article/details/gmdazonli.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxradeknc.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gnsoyqqbq.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gbrvsezii.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgxfbjfd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gxclcewyf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gkvtbrcan.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gniglvnkx.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gebrvzwpi.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gtmsljvis.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/gonhnxfun.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gpjfdqhtg.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/guyzoraks.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gypgfkitl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.yfazqb.com/Article/details/gnatmyotr.sHtML

);
来源：http://3g.fktsv.cn/Article/details/ggmnkpddu.sHtML

[Q03] 增加列
来源：http://www.m.share.yfazqb.com/Article/details/gkjxnalad.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gvihotqxd.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gatphhxpk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/gysyommqj.sHtML

[Q05] 重命名列
来源：http://read.share.fktsv.cn/Article/details/gnhmjpepx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gfsddbizk.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gwqtcjago.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.vehdjk.com/Article/details/gjqhqwqwv.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gkilwmqrz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gorkycjua.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/gjqsslugc.sHtML


<!-- 参考信息 -->