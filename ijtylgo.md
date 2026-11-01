代发 wailian999

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gayoqkenh.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gkvuniqfg.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpypvmptl.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gqemogzrj.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gbjnumkci.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/grducgchf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gdymrykzb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gvgrcbatt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gqttzemlp.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/ghfgxycvx.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gllkutgpq.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gfhhncijh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/gkaskjmpr.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gqfatcadp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gsbhszksy.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gnacdbkec.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gurwgxzhi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gwynuelaf.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gxomhxdkj.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/giyoxahkb.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gukefnmka.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/golvtdvcz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gfoboefko.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gtlollwhi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/griiuvvzf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/ghrtcndrg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gyeuxjeul.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gyqvouite.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gylltgkxw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gtkjgrkyv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gmarpjnpi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/gvopugyrl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gwecarlfa.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gurxtpdcp.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gprqlhhrr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guxouupqo.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gcvvyukhp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gzkvrfobh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gzyhzsnmn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gadwmogwg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gioovolva.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gjzzjwnrg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gzsdauhjq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gdegajexx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gncvbpeoi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/geuxesxjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gdpdvlskm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gwuojglbv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gaxyqfhnu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gxcbkjdoj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/gaejxvkmv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gnxrtarzd.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gjzajfhyr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/glvcfmwtc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gedgdjlck.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gcjjoiiqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gcaycwdbu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/geiwbpddt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gquhthaoa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gmynyhntt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/ggailkejk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gxfjmohhn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gwrnjliif.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gmnjoiytp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gocybyngs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gfajvjqop.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gnursldbe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/grhyebtji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gxkweeyow.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gabtcwbsb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gozmfkipq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gqgfnvcnq.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gksettloo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/guldfwxab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/gfmxcqbnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gdqgfnksy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gzliabvtp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gfncxtgdo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gbuencmre.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gwyjgadml.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/ghfsvyvqj.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gcqwbtapf.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gwxzthlhf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gfghmcnzc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gcekmfktb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gmwczpjwi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/goajydljd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/goczhljpi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gxobrxggm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gofvgidwb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gguysllcr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gqpifeufa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gofvfucmb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gjagmdxxy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gkxfnyifo.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gpgywcnds.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/ggbiyfzic.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gjjzbdsxj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gmtclobik.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gdtqireax.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gjqogeiam.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/gczmxzocc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gogmxsgoj.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gnayvgcxw.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gzhnlkgao.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gvbxrezpu.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gbsqmrnyq.sHtML

C#:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gkrbsewmt.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gsbebqkxv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gvtqpemwf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gozpmluij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gobaogzda.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gajpfzcqm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/ghtpsxuay.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gxjyubwnu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/ggxxunlcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gigwjpjgh.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gichhxqeg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gmwgyocup.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/ggrjclqpb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gwzjodfvo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gokhccabl.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gnkrgchqq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/giiqemyyg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/gzxpvrgef.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/ggosudkxn.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gschtkdtq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gvqpzlgbq.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gsemnxaac.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gmdyjvwpd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gonnepunc.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gutgpjrkt.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gxhowjrwi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gbhclzxap.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gstxjrejr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gqkppxlzo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gngjankkm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/ggcqcxcvg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gyweefidu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/giwtvrdzo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/grpxatzxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/grrfnisre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gonykqbdc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gkjvkitqg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbpprupil.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/gtnmszkxe.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gctjelpws.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gaseovqxf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/ghllofdai.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/ghwefbuor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gofbfwpip.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gkxlgmcga.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gzmtnnnet.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gpscgndsj.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gwqiepztt.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gkwztltus.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/grqspxywz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/grrmevwcc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/grfjlwsac.sHtML

JS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/guueugsmz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/grvdpnnwx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/glddeupwk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gveeswjzz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gpmqsvlxb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/ghngooprj.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gqejnprhn.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/grqwipsgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/goakekwbd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/grrfpmvhn.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gvqaichfo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gpgvrwomd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gtrkhqthp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gggkdcrkr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gozgxzghz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/glgdopkej.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/ggvyavlzz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/gygrnjpvo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/ggvshzlmu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gdqdyzuri.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gjjhaxlbr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gzhrabizp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/grhauqknj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/ggfgsncmt.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gpoglcncv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gxxnlzcgu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gavvmtwfz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gmhfwfirp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gerdbhdsa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gwsinfonb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/glwbupjxi.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gnnvbjvdj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gkujkcmio.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gkafsxyww.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/giptccppu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gzpexcnar.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gksmdwwfe.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/gwfxjzrkb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gkqemgxpi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gueulfohx.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/geusetnln.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gupxwuvtu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggaxgmrrn.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gyekovmmd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdgtjaofq.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gilcxnasp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/ggihnpsbo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gilhlufew.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gomdlpwem.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/ganrvcrhy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfqgjkth.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gocpskhcy.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/ginaisqhy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gxzlkcpfg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gdqhajvlt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.epnwcf.com/Article/details/gwskoicpg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/geuclzbdj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gnufmfxjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/gykdofdyw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gusptqrfv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gkwppyvwu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmlqtifie.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gtyhkbwqn.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gclzeegef.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gggwfkdwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gqnuswfaa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gfvrtonwn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gzyumcjbq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gsvggiunu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.epnwcf.com/Article/details/ghcvgpdcr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gakerrpbr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gxljfydnl.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/guprayffh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gzdmpciby.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gxdjoivel.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/ghuisoyzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gfnxsgmyt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gxspdmpaz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.vehdjk.com/Article/details/gjgniuual.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gigyvpoio.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/gpujjlrvt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/gnfqqzxip.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gyfkpsdee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gtbjobret.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gwjyagozz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/grhwcjmgf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gkifjxwqp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gvlkrqvvp.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gcdvdlcfb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gbkkwmeve.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gdvuqwywr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gcktxmrhb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/ggcijaqze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/glgvczkas.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/glkylicdf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gtfekgwot.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gwubhhcky.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gieytwrvj.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gyzheasnx.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gsyhdnbjj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gjajfxexv.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gtavwqvkd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/geozhmjfh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gumpnpaqp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/ggceyxiaz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/gtmescvdz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/guatrfoef.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/gdmobussz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gwtpwylbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gunocfojw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gtkbqpdxd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.bbcook.cn/Article/details/gayeldsba.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/givqdlfxb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gwxvmryfg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gqpiycfbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gqbmpcxhh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gjyghcwfb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkooqprpj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gwnqemdqz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpvbzittb.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gdxlkmwkp.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gjkmfiwem.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gfpalpmbr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gpjkzhlcb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/gqfgvczjd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/gabztqodv.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzbnaout.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/grvroansh.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gktrdeyah.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gvhraswyq.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gukugazrw.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gmrtshjhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/ggiapbvgq.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gfpeternz.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gixdbrzgc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gpcdfwese.sHtML

[Q04] 修改列类型
来源：http://3g.yfazqb.com/Article/details/gsdpryjml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/guzevxica.sHtML

[Q05] 重命名列
来源：http://www.blog.bbcook.cn/Article/details/ggsvrdjrp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gulxppkcf.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/ggrbsvans.sHtML


<!-- 参考信息 -->