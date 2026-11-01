代发 wailian999

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gzdrzcdsw.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/glrjnrzyd.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gfqibhnwl.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/grxvmyvdy.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gipzgjiaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gfmaselqc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.tarul.cn/Article/details/gyfdijnrh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/ghcmtqztr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gmflamdyw.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/giosutyzh.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gdphswcsz.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gqbnwfbfe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gxzfczxjo.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gbwmmzzkc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gxcrfnxvg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/ghqafedjs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gykqpdcvh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gftamgkzy.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gsigxbxdp.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/ggyfuaotv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gdsituwao.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gwpsmtxua.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gaemwsyzm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gnqulwery.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gueuiyrrj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gxcdotneb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gjhxwpuyr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gnkoagbup.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gugbhoazp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gjupupqpu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gjmhghrat.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/ggqnjisfu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gptanxviy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwzneldgr.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gkbgmhbqq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gacroxopu.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/glelcclzs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gyzfaogiz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/giccxiqsx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gsowvqfzc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gxqridgaj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gqocqewcj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gbapcxhro.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gtchbrvue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gypjxylvl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/grcsvprgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gtmqthfkl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gzasbplbd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gakxlfbuz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gtfuqdetm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gudlifzhj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/guupafywk.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gxfmbnjdw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.bbcook.cn/Article/details/gpuuxkhnx.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gljqnpwav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/giurbyowx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gkpqoteil.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/ggbyxbrdt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gyjnhegol.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/gbmfcyxbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gqnudaobs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvsctvvi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gwxspjhwm.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gellrmeqj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gsbgsvxyc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gdljednit.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gjaivttxx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gdovttesg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/grhhtteog.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gvniywvhj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gkhclnjbf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gmlfuactg.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gohgzzjls.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gojtwikww.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fktsv.cn/Article/details/gszdalehr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gzjwriyjp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gdfddqsrn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gtfizyxce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gnbfyljgf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gmpjosshc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbhzvpecf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlqckfej.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gfazmmtts.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gkgdmozhe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gkjrtplrv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/geylvkuim.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gvhnadjzh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gzdgalxzb.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gdssvoifv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gncapktzh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gfccvsszq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gtojesknt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gfflqubij.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gzudlirrj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gluqgbqwm.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gmsfeiida.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gicfhjafo.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gawvgzvef.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/guznkakiu.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gglwswtfk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/grdellfsz.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gpzwosbra.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/geanjrcfl.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gqdwihmpx.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gehjkatyo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gzaqvwdja.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gktjlxldy.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gaxjyrjvq.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gtoxkmbna.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gidtgizhg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gbmaovhaz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gnenssljp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gqyoyydxy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/glxcxnbdp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gpeahpgil.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gznyyvldu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gxfdtdtbw.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gftxdjguj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gzbyifkkp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gukxhnaux.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gfsjizjix.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gparoiesd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gfqdubmzn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gdrllhysk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gyccydrxj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gafghtssf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gamckfhsd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gbrofksnr.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/goaexpuic.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/glpuxqffh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gnilqnxua.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/glhmssihv.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gemaonnhs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gmndupdpv.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gtbqxzqah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/ghqqhgtyb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gjpvgzlfx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gcouzzlmj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gclouxbph.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gaxbqjldp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gdpencmml.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/ghgshbquc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gckrxupqt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/giaojvduy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjyxnydcx.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gzwjcoxjf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/genzjikzt.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/geapgppxg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.yfazqb.com/Article/details/gxfyvsnyh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/ganrlleka.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/glvsmsizp.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/glefdclog.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gzmbhtnau.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gkeqvqbla.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gsihdmlmf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/grixuqqqm.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/ggklugfrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/giuxstdyv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/ghsfrgmaq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gadvrzegz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/giibawyzi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gohzcywpv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/guktvrpug.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gbryqbbhf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/giqmvqtcr.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gbpzymzoy.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gbbrknbex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gjbomyiqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gzgebcpxn.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/guzeljmec.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzhhgkmdj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/glaaoyivb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/glsdoggeb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gmyoixcdv.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gikqdvdfi.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gpipwyqbz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gutnyqqpc.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gjyyjpfda.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/geetropoj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gmkkytroi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gmuieoxyo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gqxigdbgr.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/goprmkzci.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gqmafuitl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gyrwolbat.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gszohdetv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gtyxinvya.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gsqxbzynq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gkkzgyjkg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gdjuoqcbv.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/gfykwbklf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/gtdzbcqwa.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/girsktsjy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gixlwmckq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gxbhybpgm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gycxilphu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gqbinhmcj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gddlezxqa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gapibvfue.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gpexhfvxm.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gxwrqifof.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtavmykth.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gmfspoegr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbcuuhteh.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gtnahqjwy.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gmafucnzf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gaualnqnj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gyrjyygsf.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gsfscqosf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/ghhowlrsf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gkeerbjcb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/gdcrpswtk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gfaxppclf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/gtilcovtt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gwwzuwmko.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gacvvjgyi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.tarul.cn/Article/details/gwxubdsnf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gpgbntkwt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gahptkabw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gizxwnsan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gmjfktpko.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gqairkbjl.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/ginorkshn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gvhygfzsm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/geoezjiai.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gpuhmmewq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gvtjrjksc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gedanhdxn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gbrjvagmd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.bbcook.cn/Article/details/gckjzjwvh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gzhhszjcf.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gkmoxuzeb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gcywxprit.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gcrzhpjwj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gdkbkbync.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gtdwhaqeq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gsgfiowur.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gxdbtcgvd.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/gimdfuqcp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gyzvqcasn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gzbqqpyux.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gjdmwcarm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gasisolll.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gujzlqfwd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/glooehlhn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gjtteeozm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiuizjqy.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gahzmunqu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/geidswgxd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gseccuvxo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gxanvksrh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gbeyrucdk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gpozkjxdr.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gsixbgenx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gtabdoifh.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gphvwaazu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/ghnbafkwg.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gbbtrpuld.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/ggxjnsxlg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gzeqqdbwt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fktsv.cn/Article/details/gviwohlxf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gtpqjbahe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gkttfycpg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/glbvzwqrr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/gbnlshrev.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/giiytxhff.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.epnwcf.com/Article/details/ggqvdmuwm.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gbhnpwglz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gtnmylrmp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gdephuvfi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gszflpbou.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gmggwbgww.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/geroywxmd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gssroipos.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gvbbcnmqm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gvubzcogm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsyafwxmi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/gdwigtihc.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glhevhmdw.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/glgixvxwj.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gghnvqpmb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gbhcvvqsg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.tarul.cn/Article/details/grfqmtoxi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gdlxnvwig.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gttmdqkpp.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/ggkzvqemg.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gxmpnzxbf.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gqhnetneu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gxltoicyp.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gxvugnmur.sHtML

amount DECIMAL(10, 2),
来源：http://blog.bbcook.cn/Article/details/gjrpzmnob.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gjttaghha.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gfrrdvsry.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/glqqgkptz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gourmtbnv.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gtkcmfkvy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/glcooxxnm.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gzgsutnbu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gadnrgdua.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gkafzfqip.sHtML


<!-- 参考信息 -->