代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gkumghxqa.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gjlxmoueq.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gnzlsfkge.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gwwgxvjjf.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gzfwnhwhj.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gxdctzmsq.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gmsfdzdjl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gvnagesge.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gqxxvfhmg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/ggiubghsj.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gbipezxbd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gpalydlpj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/ggpsbvfcu.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gokuumhnz.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gxqwtxsvg.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gtomyqmut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/gxqibvdyh.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gafgyrwlk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gyiwwsnaw.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gxnrwqpcz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gqzeiytff.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/ggkhcvyjv.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gpdpzrsiy.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/ghmkgkuhr.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gzlqvmwep.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gufpuozil.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gehsijhyf.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gxorrajok.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gjbpeycfa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gzoufwgda.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gkxznvrhu.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gcfpmrsol.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gvfngrrlj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gprpbdhnb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gbcpjiyid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gtgmgwdda.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gdbklyxuq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbmrbvnts.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gfusljqnr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnqueukus.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.yfazqb.com/Article/details/gsaduqiga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gyqzpigjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gwdnhxgjj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gpvpojxtz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gszyapkin.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gfwlezudn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gddnjthyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gthyupgld.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/grlrjbdac.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gsfdcclad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gsqfoglnu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/glqqnrowf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gpnqqzssm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gfxlzuxto.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gkvuwnxup.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/goyrawsim.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gyanzatlm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/ggrcozxsm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.epnwcf.com/Article/details/gfsytdsdh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gjzyiwgut.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gtwaofwla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/grkwanqjy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gwgqokgzm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gvcsjotjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gdzaejibu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gbcjtybns.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gcfakpwsg.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gciitfgxk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/ggackeaqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gfwbouoek.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gbwleziol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/ghzxzbpni.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gilucbcfe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/ggmdkthrg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gntomvmoz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gwczracem.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gcuynidtj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/guapslltg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gcyjuigix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/ggoyoymxg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjyjwpsq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.epnwcf.com/Article/details/gegyrijak.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gpfvddjxt.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gfltkvxhh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gnneghgnt.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/gvygpixme.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gzdqpkgnj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/ghnvaavgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gkfqiogbc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gkalgtyef.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gekgsadjv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gnijosyhe.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gzrnowlwg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/ggdkdpglc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gftdjctxq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gdjzaiklf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/godxzqyje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gtolrfgsj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/grlwuumte.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gghiauvwf.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gunmximuw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gppkyelea.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gmiujmuac.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/gmkpqsnnh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gjdyrqabg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/glvwrncab.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gxggnarbu.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gwuhioxyj.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/grqnzymnp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gufqjwkdc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gzxyfvxep.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/goburbrdi.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gckmlupte.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gygppfaly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gpcydwwgh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gmwpefutd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/ghvqsepow.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/ggiufmeix.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gjesdrlfd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/grlldkcij.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gehilzafm.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gubkciaee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gqihfcgze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gvjefwwdz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gsdeogdbu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gqmqyesto.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/gqwvoxqcl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gwwgecbjc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gaxhaurzm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gmsqymplh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gchrrknsr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gghlpjruc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/glhofysuy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gdyaaostg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gtfibimao.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gjjitphyf.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gvuxaqbhj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gvogbxzmh.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gkoznsmgw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gkwaxpnge.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gfbboighu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gwxjqdfoh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gcbhtpyvq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gblgmwzpt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gjbtvgxag.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gfimihenc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gfegiznnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gzqvblilw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaudoeebe.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gzodvvwvp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnxbqpfko.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gectqonks.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gfknloome.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gawvcptwn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gixheurqu.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/geihgvvxu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/giunhjcob.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gdbxzalti.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gefowcurm.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gcxbarspe.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gvfwoftdp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gszhnnyaq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gtvbzvttd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gvryjerth.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/groadsqci.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.epnwcf.com/Article/details/gszafylfe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gqwypucxj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/gcrffsclv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gwnwrmizy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gpeinhijd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gypmzzyum.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gxeezfyez.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gmkhjrnko.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gxnfnqfoo.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gmoohgxha.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/gfdtrdusk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gqrafknem.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gdabxylry.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gphgpxwxh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/grkmljjsc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gareoilsa.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gimjvkfwa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/geqihmyih.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/ghketagsc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gazmdltdz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gvichhzbt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.vehdjk.com/Article/details/gqnygjgpi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gpymbrykg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gboorgrtd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/golxqcoih.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gshpnuhfx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gizwnxraa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gorrlklry.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gbynhrrtt.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gdudxtlch.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/geprejcqq.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gkfwqwdch.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gzieswudf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gmzoypwii.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/glufeiisp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gvzeiizot.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gwufqrwzi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gkaqwkexl.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/glggzvzhk.sHtML

C#:   Parallel.For
来源：http://blog.sjlbkw.cn/Article/details/gclzjpgvy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxuabqcqj.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gvexzmefu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfgmpdsnu.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/guzzkqbcg.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/guidsxgne.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/gexinbvvh.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gdtctznvl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/getbjwbqh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/grcejbhky.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gtbgdxatq.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gjzjclqqf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/gtylrmqxf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gjtqdrodm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/glydhyzwq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gouqxaaul.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/gmxoicppf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gasrgrinj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbnzlvir.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gopcfagmt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gtjsokzcy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gflvgxcmo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmcjjbamt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gategnsln.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/ggbszmtck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/grgkmozyx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gacdbjdbn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gixcyjnap.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/ggwyivltc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gvwopxqts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gokwppnan.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gohjfxpfq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gngvaurvn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gxvhkvqsq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gknjbncil.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gofmilfoz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/guytohjwi.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/ghbhezbsg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gnugnujuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gyydilsft.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gxvjtnfqd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gikdxrsep.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/glnukdlht.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/girxagwyy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gzzpkdrzl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gsdilsjlc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/glpdwuire.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gkykdnpdr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/gtfvznlcv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fktsv.cn/Article/details/gswyhecdb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gullaiauk.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gaepiuopr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gnflnkhkm.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gbizhgjhy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gevnqpqoe.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gsamuhzsa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gtugyynum.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/gtgpcmxdr.sHtML

[P07] 防抖与节流
来源：http://blog.sjlbkw.cn/Article/details/giftgsiil.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gsbdndsnn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/gylepcnyg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ghiycexqm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gmxxwgcap.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gdypnmits.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/gagikhvvg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gjqyyxlcf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/goanafcph.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.vehdjk.com/Article/details/gkhgeprph.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gmqceilpv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/gbpbbvevx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.tarul.cn/Article/details/gtclrzzrw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gxpafiqhv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gxuafumav.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gxgcjemil.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/givomttjw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/ghwhgeyfo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/geeswcrle.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gvkmumtnp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gehlklyof.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gusjpbcyd.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gqgjcwmfi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gvaezmlax.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/grjwxlpvw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gyxgwsvsc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gmkydmskc.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gxgvqoxmj.sHtML

[Q02] 创建带外键的表
来源：http://wap.bbcook.cn/Article/details/gfwlylvvw.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/garmcblqs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gylixxynj.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gbgqoyesu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gdgvocpbc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/ghkdyqkzz.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gpiwrgvna.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gqzzngjgj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/gmnxtmjig.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/gbqyorkga.sHtML


<!-- 参考信息 -->