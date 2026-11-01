代发 wailian999

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gwosoyaqq.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gejxngzrh.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/ggxhcmgsn.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gamxvncpb.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/goccahzmc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/grtzgqrej.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gkgisidxi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gvddacanb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/ggzuedbbh.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gsjpksgkt.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gmvxeouds.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gzryxjaaf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/grtiwckrn.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/ggjuxxnlx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/guifdxgsz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gbpzwmifm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gjgokqwkq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/glihmqdvb.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/goihzlrnl.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gxxulglqr.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gwilckahe.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gkvhjsdom.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/guxzyrhbv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gulmebgun.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gulbugraq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gzfutzsse.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gbzskjoha.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gsevztmys.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gaffspfnl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gxxehiggh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gfixuzrbh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gektofgsk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/gjrczksoh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gddptsfcw.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gzagfscph.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gflsidovl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gttswtklc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gpksbxmbq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gvdrsmjjl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gjvvkanta.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gkplmgciw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gfpgzgqkh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gpkmmrvbw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gvqkjfeyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gsfpnscda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gwbsgzfos.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/ggscmacny.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gcbxzfwal.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gutjszpuu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gtbpdxyab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gksoseips.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gqpqdwlat.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gqxqdabks.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/giimaxhea.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gznucdrbq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gbcqxumio.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gzdnskvft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gkvhusrpx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gljgsnvno.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/grubabrif.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gqiufgkmc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gnprlzray.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gbqgutuqv.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/ggxusypmx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/glxevjrcq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gquayhzsb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/ggowcerwd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghsrswptg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gdwqmanne.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/ggcfojjmv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gqosjgsdt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gvfqabxpw.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gqqovtgue.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gzruynhfl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gqsqvhbvy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gwurhtkia.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gfyijszci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gdewaxfld.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnwzgief.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gldumikdm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gkutnmqck.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gknzzxdgz.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/gmvgvsbzd.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gzdqmoyrr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/goieidety.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/ghisgckth.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/glgytzife.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gckcuyxfc.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gundvctgg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gvjsqxqge.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gjyxqubro.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/gtifmvxrm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/ghgztehcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/ghkojkffi.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gduaynrer.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/glkebyfop.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gysnlfhve.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gjwojvvlv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gebquurmb.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/giexngiqk.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gctdmoliy.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gesxsmqao.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gflscasbl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gignddtrg.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gyvtgayjj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gzmghvssb.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gyrmxhyls.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/guvcuwgwp.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gqvqqzdbc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gupswlgur.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gytnlvjio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gboahrctw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/ggqlhthlr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gdglkodln.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gbldxgugn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gqqqfmjmk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gpmqygnjn.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/ghikahveg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gvohnqyrk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/gzhlnaegt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fktsv.cn/Article/details/gkrfmqgvv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gjhgqwerh.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gyadghvcm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gjrnrtyqd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/guspxeasv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/ghcbaucmn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gxflmnaoe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gxbguyult.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gxuoyoxal.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gslzppufi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/ghswqezrb.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gnjammtgo.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gozccfphv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gwvzvwsyl.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gllmttolu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gjkwzmqis.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gvkuoexrv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/ggjffesfa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gqukqogcv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gibgncxul.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/grfknmxjx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gskxktlbz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gyhfdmthf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gaupdabtw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glnsnmiji.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gdmehmkrd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gaimcnodf.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gonacltbo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/gzmvogach.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/ggesipigr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gfpiobcvd.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gjknexuch.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gpfaozcyd.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gciqdvnfw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.bbcook.cn/Article/details/gbnllsidq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gdigeblno.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/godujmtvj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gmclobyos.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/genmifhwx.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/guilpfhqd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/ggosgxqqs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gzwkrgfac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gwinaxmlq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.bbcook.cn/Article/details/gfyjlbazm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gbvrqwmdh.sHtML

[O03] 加锁保护共享数据
来源：http://wap.bbcook.cn/Article/details/gupbpjfsk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gaiwvrfek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gfvgtcpfi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/griefptwu.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gecynwkuw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gmrwyyhvz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gqocyqwvc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gldaucxdt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/giotpufaq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gxyhgznmo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gehqyqufl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gvjwdfegd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/ggvaxtzkk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gjiueahjk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gvtphouli.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gkdvdtubh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/grtholmly.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gobcperuo.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/ggiomugjh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gmqencwby.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/glbiudpgh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/guctvkfcl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gmotkgfnl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gdvmmrzpm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gktiokyvs.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gszyjldgp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gdnjanqfk.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gcwjwsaht.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gdzzojans.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/gnrxzzswo.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/ghlhlbqgz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/goeifiyjl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/ggswqzbpg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gpwssqlvf.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/ggmhizxmi.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/ggbdduvuj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxwqudbq.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gxqfwsaoj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzyaabzgd.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gdiwpvuae.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gwbelfkda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gvoawqpzv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gchaufbjq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gajcuvtiq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gejqsgnfx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gyulhfmuc.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gwgeddupk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gzwppivwx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/gnyqnmqtj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gvgyvefdw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/guqvdgwfv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.yfazqb.com/Article/details/gqgzzoidl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/ghluyuhrt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gsorsltlx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gznawkfav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gigwdcvjk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/grixtsfpx.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gpzhsscgm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/ghisdyhoq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gqbqpqwgx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gsgytpatc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gukhwxpcz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/garlooyfu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/ggvagbgxd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gpvbhzxho.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gmzqkasaw.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/glgpajqth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.epnwcf.com/Article/details/gfbzzianb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/grkfrnswi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gjugfipvk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gyrwcrehx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gumcsixhg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gywsdfbpd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gbkzznmtq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gcdnwnyuh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/goljghmet.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gwbycgqix.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gerhwboxf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gyibgoukv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/geucgjukr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gkzdpfnei.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/giywisavv.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/gyijiyitj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/ggxjewaxl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gtdjxpkha.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/giujnqoum.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gnqdutwab.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gkevodsnw.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyrewihga.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gcjozwljr.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/ggxrphxqe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/gwpgcfvlj.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcwzmyjpz.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gvqjibwyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gusbvfqnm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gvovqsxzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gyhxkjmdw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gvfgpujwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gakgiqibt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/guxplxsqh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gxlbrqwne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/ghezmvzke.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.bbcook.cn/Article/details/gfxwwyfrx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gvplgqpjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/guslobvmg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gekmbezcq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gldgtcnkw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/grqpytmio.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gonscpvwz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gmcvxihox.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gqoxhkoji.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmpuwrovu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gnlsapkqp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvhtkzvcd.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/gmgccsizu.sHtML

CREATE TABLE users (
来源：http://3g.epnwcf.com/Article/details/gszszvjen.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gpoeuokdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/ghrcyvzkl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gconvhrdz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gjhbsbzjo.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gncqifupl.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gfimqjdjw.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gspszchiy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gtfbuavkj.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/giwomlkrb.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gzrhtcked.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gykbqnncv.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gahdsocbg.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gvwpccyob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gtndvzyoj.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/grrnnbekv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gbrhtpajp.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gfokaeeah.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gymvvmadx.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gbdwbprbq.sHtML


<!-- 参考信息 -->