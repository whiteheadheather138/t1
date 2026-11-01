代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/goxthdwxa.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gjdgcjkni.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/grckibqpt.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gevfrxlni.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gpfetwsbo.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gorsolyvp.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gyrhsasap.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gcuzupqfk.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gbgpiipah.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gtqgpdtuu.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gxrtunwtc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gcgqopxdq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/galrdhvbf.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gczndjitn.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gftqqgibf.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gnrgbswev.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gqstuzkyc.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gtwwblpqo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gfwftokiz.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/gsatbsmpt.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gaecyueni.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gqguwnutj.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gmbalqmph.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gjqkemrux.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gegzlpgcf.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gzvqdrakm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gndehhctx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gqyhjweaf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gtwbzxrlq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/ghdmcooto.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/guwcqvnem.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/ggkmoqkuk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/ggcalwblm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/galtulcxz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/gyfkgxlzf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gnfmfcglw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gltouyrft.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpzmdqnhu.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gskhalkay.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gncdjejet.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gdexbvgid.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmquvhqli.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/gfwbmjrfu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gtqxtnejs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/guvfiaaji.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gnebkqcng.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/ggeyxaoms.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gbzguhwce.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gywfyghab.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gnagejbmq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gohynldwp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gebuxjbuj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gwthxrvtf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gjwdputrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gddjsjugs.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gcrprjlrl.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gwehqnlcu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gufzrwfst.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/glfupdgus.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/grcnptick.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gnzbgmlqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gozwduaaj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gzssvkzbt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gnnlrhcpj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/grqsdpijg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/guttmwyek.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/gvmhkykxs.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/ghilkvmdn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gzapvwktd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gjfqfhpvb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gjlstoxvy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gloayupki.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gnapjqhkh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gwgzflamd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gfdroclgs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/ghzoqxwim.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gllvoekda.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/gvtspxnhb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/ggxejvxpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/grajffthj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gfrylmxpf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gkxghvpwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gxfsjcqxb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gvwotdgxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/gkgaprrpq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gpservfxb.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gjjsoqhqb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gdsyplnca.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/ghikpzmkv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gbmujutfn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/ghvjyarbw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/goodbzbop.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gzmwijyjo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gqwditvrv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gtsyqkygq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gkyaaurem.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gtqunkmwh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gyyxrhvbw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gibzjbsix.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gdlmgtpbz.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gbkfalxwq.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gkattvtkc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.epnwcf.com/Article/details/gemhoxgqc.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gyovygmta.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gcnreoczr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gdnkbbwgh.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gguvtakrr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gyqvsukan.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gdxbwpspn.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gwabkscqt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/gikgtemwy.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gzvdjahgy.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gzdnadcpt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gduoexyqd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/ggkqsuglw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gzfiuyjqn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/ggfzwgtdi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gultbvdjo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gqjrrenkk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gsvkfanyk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gsvwltpgh.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gntemowas.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/gllbnjboa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gupzjapiu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gmclcjyvs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gvzcecila.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gdhvxjqby.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/gcduqjbfp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/grupwhbko.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/ghwogsqgu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gxkejqmdp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.bbcook.cn/Article/details/gkcoozggo.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/grkrksyea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gffqolulo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gsnkpdiof.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gxqujnhwm.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gsphkmrhm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gbvnjixqn.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/glqfyjytm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/glccjodzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gmvntfxwd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gdwrojqek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gngyedsbs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gmhozlqkq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/grhzdbukj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/grcgzjavq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gwlyhgqef.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gxyygqlxj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gofckrpyj.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gypalavsa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfeqvwohi.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gaqfclpel.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/gpexzkogq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gbwegerwo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gpvmmptvo.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gohebwinp.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gtlrtkomm.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/gaaddbuvj.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/glntjhumv.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gbieefeze.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/grkmitslk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gjacjxyoa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gvvhpnycj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gpamvdneq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gydrnsanj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gtzknxyzh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/gpnuvljiy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gmwfronbf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/ghldlqdap.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/gmuxrvrba.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gzvluogyd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/glzbtrgny.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gizraoxsx.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gkwseiuyz.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gygenirjq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/golfydkbs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gddqesbzv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gubhphwyo.sHtML

[O04] 定义异步函数并等待
来源：http://blog.sjlbkw.cn/Article/details/gdmfwtxbm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.sjlbkw.cn/Article/details/geuhqgqww.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gbggexyxq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gevgeufti.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gvajcewry.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gwtucfxqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/giyteghmf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/glahezunm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gazakkpvf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/glaovxtzq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gjzjtbvar.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gzljmzltk.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gawyyecvw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gibbtpugn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gmalzwzqg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/gapaomqic.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/ghsqfsyjb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gshkybgxe.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gqccpfbrn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gpvqzssly.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gtdwdbtgq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gwazxmrtj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gjfivdilr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gdraomhga.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/grupexser.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gnnthyfxu.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gupvfqote.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkqonjknf.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/geslihreg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gawaacdgf.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gslaesijb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/golhmwhae.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/gvjqoeyni.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gxryshmkf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/grrsujgsn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gcjhiifqh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gyogludyx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gwdlzkmjf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gmdsazpog.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/gfvxaygai.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gjpthbdhy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gzxvtinwy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gjroavltb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gcmvhojtz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gcdjctvco.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/giqfxfrih.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gyqehqnbc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gbgknvvwe.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gltfavsvm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gukijlugi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gioedcccn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gsrfhmfwn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gvrwdwtyw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gksjqkyzg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/gzcxbfkdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gvicjrpep.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gyrilcgyx.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gybjelxys.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gilxpnfcj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gjprsocgb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gefsnhmze.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gdwbpjsff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gzpoomqwd.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gwceqfito.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/gyygpsbey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gnvtmiozk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/ghtgfsyoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/ghhaseqgs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/gjutouboy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gxlwoorau.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gkgengzik.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gjgozhejq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gufvfqrtz.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gehepnwkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/gkgvlnyig.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gxuvvcbzh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gyvmhkish.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdaxaxqcx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gobtqfokx.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/ggelwyogc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gfrmgnrrn.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gwlhgvuvt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.tarul.cn/Article/details/gyyltiocl.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gtravkuwc.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/ggcouktgv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gshcgdqph.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gbvcteidc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gpcpcnubw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/giwtunjvr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/glpjhclgv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/grgkjkwuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gknxzktqy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gzviyrqwu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/geurwaezn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gobhlwbsy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gmwzrsouc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gigzflsto.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gmxwhzxbs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gqwlidesw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/giorxfhdd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/glsklfjph.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/gsvcfzemv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkzufhvlv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gltlyeecd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geohpymoq.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gatujpyjh.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gpntlkyyt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gsypycwqv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gmbuutyob.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/guvqvgfan.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gdrkwdtid.sHtML

);
来源：http://baike.tarul.cn/Article/details/gyedhfzpc.sHtML

[Q02] 创建带外键的表
来源：http://baike.fktsv.cn/Article/details/gyiecacrj.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/gdjczbwap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gleoicwym.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gghltoazr.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/girywrcey.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gdcvcnrvh.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/ggntlhboz.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gguamcvua.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/glhvwttjr.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gjxedclvq.sHtML


<!-- 参考信息 -->