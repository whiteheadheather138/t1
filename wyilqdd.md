代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gxjzlnqkw.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gfjwmnism.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gujvdyjud.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gdideopzl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/ghhqwjtaw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gvtadgskf.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gmkaqjiti.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gsatmqdyk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/ggaustwdf.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gwqklmcyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gqtmlurfw.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gvnkpuamv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gqupqqfqj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/gbxdcmpgn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gdkltfvbv.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/ghujfzaqi.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/glymiuaih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gwzniqkcl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gwahzfgwv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gmzdqgwhq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/glesiywdq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guvtaylkj.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfunwkam.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmwgrzkzo.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gmhwbapkw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gqfdpuazv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gnqirjote.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gsmdcmnhb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gnxqewyay.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gyuvgfdmg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gbaammbci.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/goyasgnyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gtdvshgpo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gqdshjexd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gjhjqrqdr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gmqvkszvz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/goxwpwrhw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gdmdoecmy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gsdyzzflf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gskciorbh.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/godajhtug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gqufkbccf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gkcxkkccm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/glrxulphu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/glajcbids.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/ggiaodrdv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gtleujlmu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/geqeucjrt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gityzhibs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gbffxjgdp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gnhzlfkgg.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gcxfhmvef.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gkmqcjtnm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gcygtjgsv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gqpkautjs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gjbkyfqcr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gedbobwtz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gdpwupglj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gjbwnajni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gbgscncyh.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gcawujnxh.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwmyieyf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gxwcleitf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/giaqvfsze.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/grwpuoazl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gwnzerlip.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gsxurkmdu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gygbhoipt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gdrsuekeg.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gakvaiziv.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gjqxskhmw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/grslyvjrq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/goorcuuif.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/glctdkoiz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gbofwvurv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gztxrnixr.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gcyxpfukh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gonqbrnjb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gxbysadxb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gbcltrrwe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gtewvuzqu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gkcyrksfv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gismigagr.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/graggsean.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gihnxoxzt.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gogdgnqxu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gdfoluysm.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gfhzegjyt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gcnkyzshr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gxjepimet.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gogatzrpg.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gtszhdetn.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/geguokobj.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gkmmdslcf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gscljuxgy.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gnyypzkpn.sHtML

[N09] 栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gmanbdpon.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/gabwpcany.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gcupcctel.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gnwaccfye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/ghvcdkshg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gmtsuckor.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gyfsqcneq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/geughclcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gfgtwqnek.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gzjnabvlg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/gwdaniduq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gqagwghfw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/ghvlrjpwq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gpkgyknru.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gnamojolg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gtdchgwsr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.yfazqb.com/Article/details/gcuukxfbg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gvkzskgol.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/grnvyrvqd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/gdfhtwqtk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gcbnkpkmm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gjfacsmvl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gwngzzyjg.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gieitiglf.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/grlxfftwf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/ghxxzgiil.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/guxklzaya.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gnvniyfvr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gnkuteoff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/glunivqnd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gzpagznzx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gicbupied.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gqxubyhld.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gmcendkcl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gthlvcday.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gsyrcmyir.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghbeicuud.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gwfuceeuz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gupsmpjhu.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gmsmvnyhx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gutaxrbpw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gnrwkzdxk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gglyneegl.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gksxspzpi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gnlaikcyl.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gtksaqgbr.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gfmrmdlan.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gdzkrirht.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/ghooydlzf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gelcnvwbb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gfprwcgdd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/girfnyvsp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/ggyycylpx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/guudymdyj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/ghlxegyzu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gaghcowjd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/gtihycwsq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.sjlbkw.cn/Article/details/gvyynadsz.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gqrrlvree.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gydzfbbpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/ghxxqptav.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gloqjugjn.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gctagzwny.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/glomruojq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gypzknowe.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gdsyjnwok.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gnsmpmshb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gkycvqmss.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gzlufuzvl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/gqliwadrq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gblotqhag.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gsispfbrw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gmnfblkmy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gckfgaged.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/grvpaqtdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.sjlbkw.cn/Article/details/gbgwmwyzw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.tarul.cn/Article/details/grebmrukt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/gzbrwkvts.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gqttkywko.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gshgrlaus.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gxzbffuub.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/ghdjzuswu.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gkuiixexn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/ghesvuvio.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gsuijlicc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbdlcfbo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gyuiiqmsy.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gpnjpkuwg.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gvopfkknf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/ggrcrxzye.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gytkcdoff.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gcagzzyig.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gbcgielrr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmueodquj.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gxerlpzbz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzphuulcc.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gddebauak.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gvwbgursu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/githexqdc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/glfeitohi.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gcpuqmwnu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/glgzmcoxk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gmfrfueas.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/goqvynovq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gzlbgzefe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/grmbvalhc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gbzthsxps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gtwhtjxrm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gzyoqtiwy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gcdvfuvzm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/ggmmbgzjm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.tarul.cn/Article/details/gwzxzsjpy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.epnwcf.com/Article/details/guclfyjll.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/glmnwzcgi.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gbjqfhytx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gcesxygmz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gmbchaaue.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gtmnamxxj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gqqidjvfe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/grtiftegt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gxgmtwqqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gykodtepq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gyatccojs.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gfeurtgdz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.epnwcf.com/Article/details/gprobncai.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/glazvtzlk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/ghpydpsjy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gbkxlxcvw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/gadjnmqrs.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gmupgjhtc.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gustzbahw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/ghgvtfbnw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/ghvlibrfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/goyhrbtgk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gpimjytma.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gsrietxbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkjtpjmy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/getgmibow.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gjmxaxslf.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gxfutlwwg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gdbqdrita.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gcmdqwlyp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpaewdnd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/goymlzjkw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gjsjikege.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gvlxxciih.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gcccdqnwa.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gdwrvlyhn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gwkofkndi.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gqdmlwzcm.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/ggmrbqtff.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gwecmgdci.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gbsagefct.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gyuwehkbm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/geiatbhwy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gqzmbvobg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gbagqdzlw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/gaaqogdjw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/gxopixjcf.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gfcwpeccv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gtsprtdmh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.vehdjk.com/Article/details/gzezjzdhf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gmtapdarb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/geiuaxdnx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghckywqos.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gfmzrjuan.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gdmczkwzq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gsmlmjigh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjtlidzhq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/govzfiquo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwavvzxll.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gvwzszuqh.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gfuovibua.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gznqywiff.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gtxlhpugz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gieemclfm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gajglebze.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gsseqlhwt.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gydiuhkdc.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gopyfkuvq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gwgfnqtfx.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gazioufwo.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gzykcmfuv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gobkkouxh.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gvcewtzkp.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/grlrnhggj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gnhesveao.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gxiydelef.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/geedxkujv.sHtML

[Q05] 重命名列
来源：http://www.m.share.tarul.cn/Article/details/gwmqxuird.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gxjtnczda.sHtML

[Q06] 删除列
来源：http://wap.bbcook.cn/Article/details/guuruyuld.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gcuqttywk.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gcdusiylz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.tarul.cn/Article/details/gyftvkeov.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/ghbjztehv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gkimhrqca.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/ggingqlvy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gyorkjbia.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gkxfvclte.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gfagzxbye.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gbeyxlsdx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/ggnakncpp.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gahalnjqd.sHtML


<!-- 参考信息 -->