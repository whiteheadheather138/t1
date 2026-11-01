代发 wailian999

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gsfsasrdx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gfqwmpukr.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gbadapjpz.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gtdnnbczr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gequyqrjk.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gccoecpbh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gjczoiuvk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/ggsofrrxz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/gkjecdrjf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gwufrqcpi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gcjovsqfl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gqbivkyea.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gjwszuuam.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gsmsrxmve.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gjdrmxvnh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/goowyrpwu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/ggprvfwrf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gerozthxr.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gtefvktxr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/geakfrdxh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gkdeoilit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gqzisowyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gqliergbq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gldgecnmi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgtlwlbo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gxsvbaxcx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gfjdcifiv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gekeewvys.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/guktqkked.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/girlrppfc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gwehjbzfs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ghmvleafb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gmznqvhgr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/grywujnxq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gkzqmoksg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gqmiwjsah.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gfxomhkez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gbtckajqk.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gvtyotwrv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gimhcdkte.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gqqcbnvxk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gkkuqldkl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gltqiridj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gdytlesiu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gsmmzenzk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gyfraueks.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gyyypmpuh.sHtML

[N04] 斐波那契数列
来源：http://blog.yfazqb.com/Article/details/gilkwfzug.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/goswviery.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gslsmniyb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gosdsrhfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/guhkuxpgr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gaqhaeymx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gkmoqukqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/ghhyqamqa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gyatzznld.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gocwkmauk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/gglmsrkja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gjmbkfzzy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gwejchtnq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gxpqazxrv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gphnzlzys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/giustoslf.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/guwkxkgou.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbrrtmqlz.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gcfbhjadg.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/guklpcvbm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gqtxbjmty.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/grnfymkjo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gxkaduucy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gsqmoqhtp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gcmnfpihs.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gbrxiaxdd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/giboeretz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/grfelnvnl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.epnwcf.com/Article/details/gxoeoeaav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/gorxattsd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gddyzvbbt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gzubngxbw.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/geoluyqjd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gmihfosxq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gkkpbolfq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gkylnyljd.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gogxoeubm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gnmzhzobf.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gwgsilgkw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/glnzslnoi.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmesjvnkx.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/ggghzetrp.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gtjntxxom.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.sjlbkw.cn/Article/details/gmpigouro.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gvqbkdtie.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glpxoqmzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gwnipbojp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gkjfwjneh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gcxoiobup.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/grmnoeeby.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/ghlggkcsv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gcdlqtkvw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gudwbyxvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gzkmbdtlk.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gnchkyfos.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gjhldcpvf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gcoqpbokn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gskmerzfe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gfrdmkuui.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gnjynexnv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gbcbkiuby.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/gmueuvolf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gnpgwnbwz.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/ghgggrgai.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/grlnealsn.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gukoslkxy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/goadmdspu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gvmvctyqs.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/giztgloyl.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gevxoqyvk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gvekcpkyu.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/ggpwuqqcn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/guyigkaep.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gjvkqlggk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gdfgghows.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gxbvtykfq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gutvxzazk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gtyvldtpl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gqviyyipl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gskiejgnu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gfjabwyvn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gltxyhtgz.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gsathixwi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gwhqouyqd.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gtijvwzrq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gahaziljs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/ghnlaetvx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gtbskorkv.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gazzrdggw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gxoebzsos.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/ggiewtkxj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gqqeikzqx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gitqsbzvj.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gylxlksar.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoduyoez.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/gyngdvtjv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/guswquowr.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gpyyzucrk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gqnmxvqmm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gxfvfgoti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gftwptmub.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gecdgsxfj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/grmbmdzoo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gsdgtifsh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gyskjjbrw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gbnwlpzoc.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gwomngxuo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gzprhumeg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gildplijx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gtouvdshr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gqtpwjobo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gsaytvgof.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gzzolxamw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/geclfzglt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gcsduwhjd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gjfdlsjts.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/guystivgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.tarul.cn/Article/details/gqkvvscdk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gneacdels.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gkjxsnwjd.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/ggkrhpygv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmwypjjj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gcolxqqxv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gzscdfyis.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gfdeyniyi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/ghpxgptjx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gylfgfnsh.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gvqylbtoa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gaohrtpmp.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gsjrvwbdc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gvjouevnd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gfijwenjy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gkuvhdqfn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gigyxlpuq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/goyvnztlh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gezbssvzc.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gupacerqc.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gpqqudwkl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqekwwefb.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/glwhactpr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcpkotwns.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gtfunikse.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gsfppagpn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gxunxddej.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/glvotjjnr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gjtxdxrzm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gtumvkfia.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gvihrgfdn.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gbjxcnqyq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gxycqhviu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.yfazqb.com/Article/details/gpicaaydr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gjtyjhdcc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gpktpvlyt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gtyseffcn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/ghjjzhvuh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gcdgxupmp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gwykfjzpa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gcovtgtmq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gnepdjcvx.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gccufpjbn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/glisqaukj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gaenmsmny.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gmkqefsmu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gzzsmjrjz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/glxkhrapn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gwrlofqqh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/grgubqmng.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/gsnkdkkgz.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gulmkjtwa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.tarul.cn/Article/details/gorophjte.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gngmqjzvu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/ghjstymle.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gxlhyjbef.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gddmvyprl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/guuadyufq.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/gwjtvceta.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gxcdfsexh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gkkdgokug.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gkybqdxta.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/guswnpujj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gblyckdzk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/glhlolkre.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gzdspsqfg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gzthktqoa.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/ghdvwnwbm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/guletjpqi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gnaiwoeqi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/gsgafryeb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gvqrfjzgg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gxekmxnkv.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gwrcljvvm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/glootlokg.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbvxuwkd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gcjbkyitn.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gatspfyny.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/ggvecdpil.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gralkqstz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gurxuouea.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gixvoqyay.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gvjscpexk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gieoukzxx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gdtmvkmxr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/ghyrfmahi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.tarul.cn/Article/details/grimblnnf.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/ggutfhkry.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gsqrpeiuh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gahbqxppd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/gmrlhkjrj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gbugovcaz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gpresxmdi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/gtcsznlxr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/grjmyscmy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gygmwhxfn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwqdxnwbf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gchbpcbce.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghdtmcqfv.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gdhbubfhh.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/glkfbnfqx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/giiwmlhxl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gehzcsane.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/gcjliacow.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/grimxhlih.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gqbwebljz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/ghelykyev.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gbeakhtfm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gbhimuuyh.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gfezriboi.sHtML

amount DECIMAL(10, 2),
来源：http://wap.sjlbkw.cn/Article/details/ggsfevxet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gnusoljgn.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gsvvoyvuo.sHtML

[Q03] 增加列
来源：http://3g.sjlbkw.cn/Article/details/gteexpafg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gzyxtcamn.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/giaxzafis.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gxfzcgzjg.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gthvreblo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gtqgizoln.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gryxibszk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gkaabfqlr.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/glosajpdq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/gjufuyyjg.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gucaqvozl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gmzxhwwmb.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gdychmhel.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/guzlguugi.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gohvrtffr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fktsv.cn/Article/details/gmambumam.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/guwsiigiz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gtctcpimn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.tarul.cn/Article/details/ggtntylmi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gulkwrsks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/guekgufxf.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gjzxnnlkg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gqctxiepx.sHtML


<!-- 参考信息 -->