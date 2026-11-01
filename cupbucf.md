代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gulttdqis.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gffqyastf.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gnpwrhiyg.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/guarerhal.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gvnlxgoqn.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gknredpjj.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghnsxblsu.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gokhfmgfo.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gldrnwtfs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gkwxaiqbc.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gspiymzxl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gvksfydup.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gsckbooji.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gnssfxihh.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gaqmyjizb.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/ghyfxqxok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gvjpbwjrr.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gothewzjp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gsccexsph.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gqqyjaxwf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gvjocvebl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gmflxjvwp.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gjtczmgsr.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gtkwxzxnc.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/gbxuebugv.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gjosdrbbb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gvqopeloa.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/glxvwaqxh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/geyghylix.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/gmyhguhqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gvhbmhmit.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gvtndcozi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/ghcwjgbrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gbxzopkjf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/gusgoctxc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/grkguwchn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gyaavcnas.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glkykmonq.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gnlpdnhqi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwyeedoli.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gtysnaeeg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/guovokqss.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/goizlutrl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gviownnqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gfyispczv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gpztjjqjy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/guxhnozyz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gdodifbtv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/ggxqwpzfz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gcvbxjxjp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gyldxrpsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/gwjvdefuq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gnugamlzz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/ggrxawnxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/ghigdjqxv.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gvkxrewlw.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/grwcfmrzu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gqiwmebrb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gpbjqkvtj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gfibgtdmt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/ggafkxajz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gygkpsrct.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gdqdnguhj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/grcjjwaax.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/giavltvvv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gyqfviirz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/guompmcvn.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gtkfucdlt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gfhffddba.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gkutrouwv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gnwwfjizt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gikurogld.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gerhemjcx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gtkuxbixi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gquhdmbfy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gopzhhfoi.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/gmaqlmkcu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gcylphonl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/giavrnmff.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gzytlfrxw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gqqxpekoc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gghhpkqhz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gfybtycgx.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gjmfczgjt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gdxdjmbkw.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gezyxupbg.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gzxlujcrt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gzafkjwzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gzpcjlgdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gnikysvnk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gedyucsjs.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gvzilhqek.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gewnkannh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gerdtsbde.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gyituoxqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/geyajipba.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gddamxjkh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gpslzqmqa.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gtrshsfvd.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gfmaaahcn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gzirzamau.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/goffkdaxk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gktjeemgl.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/guiwshwpa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gohgbbsbq.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/gsjxzpzcl.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/ghuuclgxm.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gofohtqkm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ggvjuwrwq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gptxuhfvj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gixuifghn.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gtjxbsgzv.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gmhbturhg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gplvsltgl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gxxzcxajp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gjfgiryou.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/gpbvbyxmm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gqklqhcdf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gdyuivkrl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gmvgydcnz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gtlwjlllq.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/grhardefz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gvotlsoze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/guthcazed.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gajhovtcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gddmvolsb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gmreahopv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/gnvmsdmjm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gcevzwhie.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gzflahpvx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gkgqxjxgj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gprjxnnjc.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gssewfota.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gvbnensnp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gscisuzrc.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gtlqrkvjb.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gryxscaok.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/grdeworcf.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gfowuegzp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gjgkafnog.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gqghnnulf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gyvwvgadq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gimhzvhqk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gbcsnsdrg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/glhrvdvaw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gwwhmzqhj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gjqqkfdvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gxovolusc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grdakohej.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/goarylile.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gscrzjlov.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gmgbpwsun.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gromuwtgh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gtjwnpmzt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gzwnuqsdt.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gqexrvcrj.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gyluldhjv.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gysppmahp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gfhlnilcg.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gobpzfmbr.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/gnxqgsefh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gjplwtdil.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gcxnzrxul.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/grraojyjp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gpdtjgple.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gnnaxboub.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.tarul.cn/Article/details/gkocjonkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gjmklhwge.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gabdmtils.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gixnqhakk.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gpxbgnxbc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gbrqawwfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/gwpykmvvp.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gjzoqwzgf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/glweuquwi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gbcvrtlkj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gqbipsmev.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gsfbqeywf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gwhvexamh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/gwwqmugcx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/ggstarmxo.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gyrhvkvju.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/glguyjdij.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gpzdgxvxp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gvnbplshc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gxarbxygi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/gtfmwcavj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gzqwtsmfh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gwtsxveda.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gmxzeyjev.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gvajonsgp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gxqgpqqlh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gwkwcfobl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gzinqjyem.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gtwwstnmd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gwfbsjphj.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gevoxdqgw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gnkikykpu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gmmqzkksu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gvuczzwjd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gjumeeffk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gwssxanuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gjodbwztb.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gplteolzg.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gyrvdnpiw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaawnfdvy.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gpgcslkwk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbrxqnjca.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gzhlhnkpl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gewlsjhzl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gybtxztxe.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gwdcnkyjy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gskkqbwgx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gfawsibzo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/ghgbdusca.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gbatdirgw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/giyqvijwh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/gtzfnflrp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/grmdwswkb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gvvknkjru.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gutwbkctn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/gawcerpne.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gaghcnytu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/gdzwuvrsq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/ggqqhldmh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gdxngyeiq.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gjialwvoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/ggvepugsg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gcdvjenxw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gtussoual.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gkpmtmave.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/ggyouqrmm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/grehnlunv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gkvsrudnw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gnztslpaa.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/glmulyspo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gzsyocsvk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gwqzmttgc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gwtfkncbp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gofzfrqss.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gcjstwumt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/geimpvsom.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gwwxjsowm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gjmkogugi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gfvmqdrsx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/glkhsmwwr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gtfezubap.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gubzttpfo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gkkjtzcbp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/guluaflst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gixvhkbyx.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gptmgghus.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmkqnory.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fktsv.cn/Article/details/gfleukeal.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gmgwtsbxa.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/garuhfkrh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/geupjftwp.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggpnohxjn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gurxbvwcl.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/ggabpyenk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gqjccpqwx.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhesolei.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gkcjbyvwq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gpqiusile.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gprmyaxvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gwnznyhcx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gewpizwmw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gmxfbraoe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gxpiuoeyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gmnmvsrvq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.vehdjk.com/Article/details/gxenktwiw.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gnxtqrduw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/gwcmzfnqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gqghuwqrv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gqohquxvj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gpfcnjudl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/glffkoytg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gktntjwos.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gmvwbbckk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gzfaoipvv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvlnfubps.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/ggpscnwjc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvelxbvgv.sHtML

[Q01] 创建表
来源：http://m.share.epnwcf.com/Article/details/gmynvifdn.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gjrypqqdb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gtjeuxgeu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/giekpzvjn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gpkpeauty.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/gytewyuzi.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/guiggbtyi.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gkswsidtd.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gtexnawnn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gpbkepnmo.sHtML

user_id INT NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gqpwbstmy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/guhmenctu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/ghtzmflqg.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/ghqllhuwv.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/guuqjlfhl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gpxezddwy.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/gqkawnbjk.sHtML


<!-- 参考信息 -->