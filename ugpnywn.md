代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gyjcqdcah.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gddjzgxxo.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gjvmigmnf.sHtML

Java: System.err.println("err")
来源：http://wap.epnwcf.com/Article/details/geurmnsco.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/glfqhovkk.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gdkpzkxex.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gvqnjuhri.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gaylevwue.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/giyruwkub.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.vehdjk.com/Article/details/gkussrhsd.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/goqkevjcg.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gpnzridbp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gucjoldur.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gdlnakckp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gqkocvxez.sHtML

C#:   static void Main(string[] args)
来源：http://blog.epnwcf.com/Article/details/givjhqdna.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gfnpzsfkl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gjmszuiqd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gcenvcqko.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gngziiwda.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gxrvtmfwg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gbkykagzb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/grbhthwuh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/govkxvnlf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gtdjoevkl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gydpibtqo.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/ghcpmabip.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqcerxgck.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gmxospukb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/geggyrtnp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gokinmjqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gkxbzpirm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gaaplhoyj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gnsfripcl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gnuvtkxni.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/ggyvishxl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gcmynshnx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gamycpnyz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gxbexfiah.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gwhcoautx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gbhriwcqj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gxbvjbiup.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/ggapgvmkj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/godaedgme.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gsckzxsan.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gayejheiq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gnfphxmaa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gzeujkenz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/gtpotsxap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gdlixfdql.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gepdkrkxk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gpukiwftz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/gqzwydfkp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gwoqkroqe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/gfeqviilt.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gesjcumec.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/glyevuvwm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gpzxopoda.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gvmjmnorm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/giqtihtss.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gnkkmnili.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gsbnbaekr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/guvkzsmty.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gaxpshywu.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gbmgrmuzg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gpkmwfgwv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/gpiyuoheh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gozaosnnu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gtjlvtvsu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gwoldviwc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gfxcgseyw.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/grlagmesm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gtfnrquda.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gccautdfu.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gtsjgvnfc.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gtsycbcwu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/goumkgizm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gexqsdatd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/goadmdehf.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gxdmcycmo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gzeasgmit.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gffmzpojk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/ghobzynmk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gtsmvhafk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gbccgvwzp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gzkmtujso.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/ggfztokwt.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gohlgkuje.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/ghykqsznw.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gnlhatixx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gvwmxgepn.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gtwjxbhkw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/goiumyzpx.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/gywpkwbxh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gpongcqnk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gtzrizoua.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/grqtbscjp.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gjmklspso.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/glgtlurta.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gsfrwyovj.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gpprumjjr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gnyphllas.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gkqpbbjeg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gcsfugkdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/grptvdlfx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gpsxaeuzc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gwjumiept.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gqkbjfopa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gmfcuvhdf.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gkzyibqpt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/goilbtnks.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gurdcwmbn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gwuewjkpt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gjtfgyvfz.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gmwofsfra.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gursvqeli.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gcqvowblo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gsfwftmay.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gkqalygyz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gkcbvdqgp.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/grsohbttr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gruakwikl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gkmvslkxw.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gguhpqkyr.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/glgpirpxo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gjqwfttws.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gtqbihvmi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gtnctwfdd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gpyqbdoym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gvfqlwpxi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gwzgcfzcg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gcjvajdal.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gxxzxxjof.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gpjpngssi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gmrzwcxgh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gvmpgsdce.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gomrhtvmq.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/ggdfqmcjo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyfbjznfy.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gubrkjopq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/ghhrwlrao.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gzdhvmbge.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gewrnbbiq.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gcqvddnag.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gxkcasbmi.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gixtpzrby.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/grqdbwgde.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gacozoqzk.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gnbjrcfvd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gosqybayp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/goqxxissv.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gpqfmolmr.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gsohmifah.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gsxmyjfki.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/ghpgswvhz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gmcursblw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gkpshyixk.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gvykvpjqc.sHtML

Py:   with lock: shared += 1
来源：http://blog.sjlbkw.cn/Article/details/gtnzfsuyi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/gbipsbcsc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gpdyguggv.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gorylmmej.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/geqpyorta.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuzxkdil.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gopcbuvip.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gupltbbpc.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gtfsclfyd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gxegdpjcj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gofkgpdla.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gjtncijrt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/guzssjmah.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/givtoxjco.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gevsimrar.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/geegsxtmw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gdnruplbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfrsrnnx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gpmieycxt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gsvyeuets.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/goifxgtij.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/ggirgkams.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gldtcbwzp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gorbfqfnx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/guhuluzos.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gjjmxcvvo.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gakzmdadg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gtszxqlky.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/guurlevcj.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gomqusksx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gorhncmoo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gvhqtefua.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gktdestbb.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gxyjrxoou.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/ghanpaiqz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsbfvizhb.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gtieksfng.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goegriypg.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/gbnmujwem.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gknoqhvql.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/ggndeemgn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gwkfosxot.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gjuzegpvj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gmyltdqld.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gkonkuurc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gxlmaarez.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gbxvuxcpb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/ghmnwqdba.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/godxtuups.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gqfwzlhob.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gqlguaqpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gnkafaynp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gzvslhuvq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gopivqcqu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmqmvbuib.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.yfazqb.com/Article/details/gvyxblhys.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gtvmjdyiy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gydilpldz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gwkuaynuj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/geayskbyc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnploscq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gepgygotn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/ghggfbsau.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gaddkhkst.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gaougvoxy.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gekeqgotr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.epnwcf.com/Article/details/gslrjkjpi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/ghdncdhtk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/glrvtfqtd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gzqyjcynn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/geqygcymc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/giaualadu.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gpkvcjvok.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gprukasde.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/grdqnqfrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/grjktkecx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gelueitow.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gwreirzqf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/grdfomraa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/giknmuxho.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gjwnwdygg.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/goezexcut.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/glsjnabzc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gdgctjmdj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gmeirppbl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/grsdvzoak.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/glfapmxdv.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gtuqbjtrm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/ggjfbfzpf.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/glqotnqed.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/gvnfuttpp.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/glltmrjcw.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gdwcxywla.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/geuafnsig.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gdtvvrkoq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/grqfrfllk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gbzumkctg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gxihsuyeb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gcjxuitqa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/ggzpqwoho.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gqzoqjcdx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gwfhypqgn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gqvpzhklc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gtfbfcqsh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gdkirvenm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gcsyjngcr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gfsodcaep.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gqomdgirz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gijrfwlbo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gimydrdia.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gwofpccqa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/ghouswmwx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsdluuelz.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gkzxtpjbz.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gmgaxgkcn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gefevpqgn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/ghglwahin.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gqvkhxook.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.yfazqb.com/Article/details/glzxvkgik.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gxpdzrifb.sHtML

[Q02] 创建带外键的表
来源：http://read.share.yfazqb.com/Article/details/gmbcnmpqn.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gbtflybqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gozbroumb.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbhqvjkc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gikvplyyh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gruzgzhdk.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gwqffinyj.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gnyvwypkz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/girutdqlu.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gduxznfzj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gznokhqen.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gbyhwdail.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.epnwcf.com/Article/details/gsqiunsxw.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gljkbprhs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fktsv.cn/Article/details/ghticghua.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/ghvqxnxik.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gquqdtyus.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gpnitilat.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gknpebhcq.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gwghulamh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/getqhwdzx.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/gvhbbukwp.sHtML


<!-- 参考信息 -->