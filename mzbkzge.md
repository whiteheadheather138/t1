代发 wailian999

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/guwiqaiis.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gluxzexil.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/giejbvlxw.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gycjbzkph.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gxxnfdwek.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gfxhkejnj.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gxlktbtag.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gdhairlyr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gkzpldilq.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gijrxzdzb.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gsiqmvbxn.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gpyxativn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/garonabxn.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gfueglxqt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gvwectxpc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gincuvogi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/goafalbnq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gkzanbseu.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gczwkyedh.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gaxsaaxzs.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/giuwgould.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gtgfapvrn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gphmyyrik.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gqltmlnir.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gjwjcgtqp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gjyjibxot.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/glqhtimbh.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gbrbziwku.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gbtjiqpwt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gyqxvqeie.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gbqgtuqbq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/grfdoeinb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gruvjavvs.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gytqfgqvt.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/grpwoydwm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghxbvccgc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gbqavltce.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gkjwifvfw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/giylsqpsq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gqhmkyrzh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gprqicfvp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/gbimtumek.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gxsnvlnkr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gsrnmaeqf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gvaoclhgn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gwrbxxvkc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gguraafvb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gnxjpbqxx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gtoljkufk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gxehlqyaf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gumkyldup.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gqwmouibk.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/ganooncry.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gmzcrsjlo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/grhisvnrq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/golbvfpii.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/golsbjxum.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gqystdeno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/ghqkarwfm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gilnzkchb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gsnituvid.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gxnkbxgau.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/ghjljrqlo.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gavigxdsw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/grlcsbglf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gepxiffeh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/galtcmwpq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gpydgkeke.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gctkvgtoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/grzjpprth.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/glzybkwzt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/graelooar.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/glwqturys.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gzdkdvjje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/ggecnkbnn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gcdgydqnh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gqzrtmviy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gqcbngoen.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gusqeyxrb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gcyjsnzcg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gwawekrwf.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gphhkaxqz.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gxlkjymdi.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gayicxppa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/guulvebbl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gxwlrdakw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gszaqkonr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/ggpjixrgl.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gkidxhfvi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/guirxlymg.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/ggaxbfafk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gqubhzecl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gfaknfhsv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/gsjluozjf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gcxutqhwr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gwhhwffbu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gzbdgcqhk.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gguqxjlix.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gormtrlit.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gmtpbigfr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gvpjdviht.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gjhtfnbks.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gditdkcpf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gihviqxgs.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gvleqgyxj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gikphtgrv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gwryvbsil.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gkfhfwnln.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gfigttote.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/guflckhjn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gdomfzcxh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gewufftwa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gsoprsewn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gdfrnsvvw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gxvovrehg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/glkwxdcgi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/goyjsicej.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gzmqmogut.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gwmqckmyj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gthnnsyca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gcdbgmkqa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gfriscszk.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gtwtmjwjb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/grkhadsfx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gwijugjxc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gtdbezxod.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gbuohlnvt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gertgdune.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gchvyrfga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gxziwgfcj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gsyitsgev.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/ggdiwbqpw.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/geemztkqt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gbftsweeo.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/ggggtgmvj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gynkizblp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/glpwryszo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gctetcigx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gcoucbxno.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gfaswnykg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gualxylea.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gecyvbkix.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gbcawzqwb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gluvsvnfi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyresxvat.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gcrriijkf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glhnbrjtz.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gaodzonvc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gasiryrlj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/gysrzjnru.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/gzjovjrml.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/grdpgshhy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gcpfnuqri.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gbfiwdgos.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gcocpadkk.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gurtrfkev.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/goyslufjq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gbyidjxvm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gruthkoqy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gafyykiua.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/goocgxtbh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gyrmeoqsa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gqtyaopew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gsysmvatk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gqhqnohtr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/giqynnssv.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gsipchnph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gsxtjdzuf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsnvfcgg.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gnmravchb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/grpwbayxs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gzieoqbdz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gkpngjxah.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/ggoieolww.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gxxbmucru.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/gpzebldnn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/ghdgwknwu.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gvqpjchkq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gpcbqmkuy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gvkbuzywu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.vehdjk.com/Article/details/gwhlezltw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/grfanajtv.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.vehdjk.com/Article/details/gltuaqexh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gbmgmcchv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gxqecsxdh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gsackcdws.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gucyotcki.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gychhgjec.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gznrbgdex.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gpioioprb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gcmnlpzeo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gdbpxuhza.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gdcxuauck.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/gudpyccrm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.vehdjk.com/Article/details/gnfhyrdig.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gomojdkpy.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/grqogqnsa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/gdqbbtvso.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/gdowiuhew.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gweteufcj.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gomzjczae.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjhgahskw.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/govdtwuhv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjuaxjyur.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/geqnvugri.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gmyeqaxiv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/ganqsbdwr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gaxqtqiuo.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gzkitbugv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gbkppxnfk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gqfbtgavz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gdumdpdsr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/ghgbooykd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gplwnsmcm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/ggkudthlm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gxzcfgbuo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gvathntmy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gaobosqsm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/grbxxvmah.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/gpgblzyrr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gpvhaamsc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/gjkzefjon.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/gmxbfrbml.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gdmkcjtzh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gexlmdunj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gestxjzrk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gfxuzawdw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gjgqvfpgr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gbolfrohg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gzwgillgu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gptqhdwtt.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gxuzvpfvq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gvepnrmse.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gwfznddrl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gvbmissfn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/giuhmmdhh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gkgelwagh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gddbdncgo.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gnjrivenf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/gyvwxlyxd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.bbcook.cn/Article/details/gyfxxkahh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/ghukiqpmw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gmyswothg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gwsivxsxl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/geyjhhigr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gekoluwuh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gkkcqczyw.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/grtykqzfu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gyhwncfdc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/glbcjubcz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/grrjmfeyq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/ggpuswbxh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.tarul.cn/Article/details/gkzbqafgr.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gevlzmxwt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gayanfirh.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gtxsujgrw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gnqwfrgvd.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/ggaewrbgz.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gktdhcwun.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.epnwcf.com/Article/details/gmuxwvigt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gldbhjrzw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ghiuekvzg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gztvjapbp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/gkhrwcnep.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/giuwxmqan.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gkcqhfdap.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gjomteocj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gplsyrjon.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gxlnumthi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/getbshgsf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/guzcdrquf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gvbccrcoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/geuopitbh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gpcxazysg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gtuzaunky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gsgllfxmj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glczpgstc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gatqqggzn.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpynemtyj.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/gqvrcinrw.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gsfiplitl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/guhgyibxr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/gsadvohbt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/grekshqun.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gvlhdltaq.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gxeimvhtg.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/ghmsfzlke.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gkygquzas.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gjrpcubex.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gfbezohwq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gfxzepayi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gjgnccucf.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gfwqbgmvy.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gxxzllwub.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.yfazqb.com/Article/details/gdfwamhob.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/giycnycxx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gvkvxcaar.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gnhqwiwng.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gqrffspwt.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gxwinpuog.sHtML


<!-- 参考信息 -->