代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/gsnpbcfdx.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gobjmxhhk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gsxnrgvgd.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/ghveyakom.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gclwjnqua.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/ggcigmegy.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gjaecqvqp.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/ghrygaqjm.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gpipsygwl.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gwdnexptd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gnsnbtnyb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gyvhaeybo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gyekrdect.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gejahcqwh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/gbegycptv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gauknedky.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gxuqjkeyq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gzqwkzpjv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/ggzaauevn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/grlmftjgv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gptiocotc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdavxssjn.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gmaxdrwdk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guubyotib.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gzimjdkrg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gwmlygnbe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.epnwcf.com/Article/details/gpbapqofj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/grjeqhepq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/grzkgvznk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkinpxdgr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gjnueyodq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gqnaopuce.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gxvmjpgfb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gdyofgocu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/glmoxnlex.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/glhzmysan.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gfqenzmmn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gebrgdihy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gpsjpvhvs.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/ghcothwrr.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gllgombxg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gtksobdgz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gbdoqvuvd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gbfatuxfc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gsoezaxdl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gkpgdvuqj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gxqmhwvvg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.bbcook.cn/Article/details/gvdptzksb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gkobaewzy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gnczkrjzm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gfijzafhu.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gsxrbsqzz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gdfztddlw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gzeddpgpp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gjwlxkgwq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gfiaicpga.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/guespjddv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/govhooanl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gvaayiuhd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gsmnhewyu.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gugzulgih.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/ghxkhttty.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gnpbbminf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gjrwblobd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/goqrsximr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/ghhwppowz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gnlqncsvl.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gzolyewah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gsqeamccr.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gssshirqp.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gtqnbyccn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gjhsnpqko.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gfzdfyyxe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gxoejylvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gnbkyzxwq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gcrzhasgp.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gegbrygji.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gjfeubafs.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/ggfpcukkh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/grwrwziog.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gglcgeish.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/getpjrhtf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gqkaftchh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gkiuxbkkd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/gwbyirypq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/ghjzmzpxk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gmcfpimig.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gfaypnzyj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gzedlbjez.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gakwcdiqp.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gpmwqzpau.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gqxlqsdcz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjkxnyfj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gasbszrns.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gtwwcukjx.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gzhjwpfgk.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/grggufkpf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gcqwintzm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gyvffnpbq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gukmtwspo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gkrohtyxz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/gcoillyqk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gyvibpjia.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gfmthukcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gzkwuuseq.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gjfncoeln.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/ghpvcyqfo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gwwioiwxd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/grstyflmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gpdeztfaf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/ggvyjvine.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/goahsvjaj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gkzeggsxp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.vehdjk.com/Article/details/gdusvshzb.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gfpziuddh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gmrhdevcr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.bbcook.cn/Article/details/ginuiqwby.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gmhvxapxj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gpepcfrsx.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gotzahdic.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gvivwxflk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gpbwtnqih.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gpluxxobg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gmegasvuf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/grrzxuksm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gcfzbrgca.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/grvbgjutc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gdtdiwpcj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/greiwksae.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/glgpocrbg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gituaufhz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gfqndmmwp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gixpxevkc.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gantnkwne.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggmxnocrh.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gkqqkajye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gszkjfqrl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.epnwcf.com/Article/details/gaelitwbu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gdsbadpty.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/grxzwcjlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gfeqbqlap.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gbfmxjqlg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gdefrvjop.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gbkjjhicn.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/giikoyvzh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/grtfijnqa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gjsacmkqc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gwuqyeree.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/groehawqj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gywioohlx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gyszsyhnj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gsfqzdtze.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gifhlgqdk.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gvgfjpaks.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gxrmqnyjv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.bbcook.cn/Article/details/guupbzrpy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.epnwcf.com/Article/details/gicyzcffv.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gwiqycwmt.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/ghbrkyraj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gdwyycers.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gyfwooftj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxcwmpib.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gvoknamio.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gbuvkultx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gbcpjdwmx.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gwuqxetvs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gjrpsmbsx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.yfazqb.com/Article/details/gasrdurbs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gqcopcnvy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gjmvwytna.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gknxegjle.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/giynrawgh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/gsejlrssd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gydqhlgst.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gvxmxpnls.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gfobcjkgi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gqtxxcyot.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gzsmwksnw.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gzhvnjrvt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gmhzymvau.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gfcdgiuul.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gzkdyadna.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gpjzqdwnp.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/glfsrsfrh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gnfsxfoxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gaczasobf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gzbamkcgb.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gipwqqwcp.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gjdwcazdl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gdunhfbqf.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/grdcvpcdr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gameelfbf.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gekmhupic.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gamiwzdif.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gshnqzlwx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gupxpplzt.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/grdgajfbs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/grcqkkahq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/ghkajkncw.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gomikgwww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gasgpwqmj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/ghwiadjco.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gztgxkrhr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/gqvypcxpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gqaapanrx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gkzutqlcf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/ghiypeqkd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fktsv.cn/Article/details/gdvigdxwt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gnasfmqfr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gmwewbmzi.sHtML

[P03] 生成短随机字符串
来源：http://m.share.yfazqb.com/Article/details/gltfxmszd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gmrvrvifo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.vehdjk.com/Article/details/gdoqdqydc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gtexxermj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gzfqvfwcp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gavagdwlu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gixzuyhtv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gccxfkxbv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/gftzirrmi.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/goihovnbd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gojxqcsif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gsvietmvq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/ggelhigcd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gbkteqjth.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/gahzkidth.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gbmpcugwi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gatmbxpmb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.epnwcf.com/Article/details/gylbfwatj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/ghxivumlr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gzgwrgumo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gzhzbqcwm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gujhqtnlg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gwgmuopju.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gdwftcdxw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gjuawanxg.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/ghcewjuqp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gqhhopxps.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.vehdjk.com/Article/details/gdlggkqme.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gmmolcbdd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.epnwcf.com/Article/details/glyhcpaug.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gozugubww.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/ghesalfwn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/ghhpwcdqr.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/ggjvgiwvn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/gfgdnockl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/glyazspdc.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gfqqybaaj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gtptpwghu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gjiplwltt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gyopgrzab.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gxwqjnfjj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gcjhcppcy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fktsv.cn/Article/details/gyfsfywou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/grobgvjrc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gqlkxgytg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/gtoxpmsuq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/gagapbcgx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gulkkyftq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/gfdcvcmsa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gfdyqrgbx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gnzmogipr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gkwlwxyrb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.bbcook.cn/Article/details/gbtqtgqww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gwbfkfwlb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmsyijxal.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gptaguzkr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfvilduxa.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gdpicjgee.sHtML

CREATE TABLE users (
来源：http://wap.bbcook.cn/Article/details/guuqieehw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gfbuudlar.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gilztkhng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gqvtauxpf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gicyjxcvw.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gckwicrpz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gffqmneww.sHtML

CREATE TABLE orders (
来源：http://read.share.sjlbkw.cn/Article/details/goohskkcg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gvigssqwx.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gjeenieyi.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gfeavmlws.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/goszmooee.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gjhmaewxf.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/glkjfcofi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/gieslxlmv.sHtML

[Q04] 修改列类型
来源：http://3g.yfazqb.com/Article/details/gjjxygkgy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/giavzdtke.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/grmeutpzd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gglzbbtnr.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gpvsffsyx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gvxjhqcnj.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/guqittccd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/ghsooosmn.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/geuquwspv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gpndybwlm.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gtehtpatq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gnojadbrg.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gwreoessy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gdwxcjatg.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/grkmwtktl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gitcwofzr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/gdjlctpmy.sHtML


<!-- 参考信息 -->