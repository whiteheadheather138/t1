代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gfwmooill.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gksfdozup.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gkqjqxjzh.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gsqzxaoek.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gupvetgsb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/guhkdgebc.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/grzzhbhra.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/goyrhvyol.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/goguumwsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/ggtfwlekl.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/graaoydgb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gzrtawaku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzwppsmz.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gmirvupqd.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/glpzggxau.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gfvceuhrr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gwoqaunds.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/gbqdokrbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gzifvijib.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gfkxjrtrb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gzkzazjfv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gfyfsmcdf.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gkufgpugo.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gnxnmdbrf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gojjmbdhk.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gwjvcboft.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gnkdwlojb.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/giowouxqd.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gtkubclri.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gccfosqna.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gontkhnsz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gnzqwbpyx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gpslluodv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gjgokvqtq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gjfcczthj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gqfjlrpqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gskolpjwv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdkmpakvc.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/goqiosdmh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkldnxyvz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.sjlbkw.cn/Article/details/gyboepwig.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gktybcalg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gkjnqupyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gukbquyqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gfaqqpxkx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gocekfhnt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gphkwbkqa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.yfazqb.com/Article/details/gglmtkifl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/guzihfaxv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gwmkrmdrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gowltnwxz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/ggtzigrei.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gwzcrcbeg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gecpfhzop.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gtcqaoxxw.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/guybjyabe.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/glfniuwgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gvpzimjii.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gbgumkgqc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gckxjigto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gdawqhift.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gzlcazxny.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gaqtslrtw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/ggvyewgkm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/goktihpld.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gshqjsuti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/ghrqooxja.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gexnzokax.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gmiuhlpdw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gaakkzdtb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/giuypevhj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gzdogofdr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gbdppagug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gmqpiwgdj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gmyxybewi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gflaklmcf.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gmjffrqth.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/ggibymflv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgbdwaen.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gicqkifvg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gjduptwhx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/geucuszqk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gdfqyhydf.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gfmithndv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gmwwoevou.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gsgcmhwgb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/giotrfhiy.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gotwfcrjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gepnxamij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gzeeufezp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/guvzpnhod.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gexsnptvo.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gktjmlfuj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/glwakctyo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gzjxnmmmg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/gsbrdlccg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/gpheguofe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/ghfaenuzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gikzmelef.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gafgbfitm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/ggmmlvnff.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gibdoyytk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gxjgbplci.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gxzmqjcba.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gwpyedtyk.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gpeuclltl.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gvfcwkwuv.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/giajqxumg.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/goujkpowa.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ghywzoyhw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gglxavrhe.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gcjdogrtg.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gyweaandq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gkpbpxhan.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/ghqbespkv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gwxodgfoy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/ghaoxmgdc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gkndrurpf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gynwjhbro.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gkufptzjf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/geecqzler.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/guiqcdyeu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gujqubctb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gzoxanbdh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gjeqssoay.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/ghaigzfks.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gtvardcve.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gabdzgbzo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gsluwuzaz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gryontcyh.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gqtvpgybv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gptlybhla.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gjpooxnen.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/guaolrxex.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gxcfrtsyb.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gfbpqpopi.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gzahityob.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gcdeffzyf.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gpmcyaxwb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gikcluxus.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gkdbqldrn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gdxorjwju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gcyaanjcn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gralfigji.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/givwdxlun.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gyyuojcat.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gdpygevkv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gteciurnd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gatpufnsk.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gnuklciag.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzhujxkag.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gkfzaqsds.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/gegbivxbc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.epnwcf.com/Article/details/gfosnmgzw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gznocjhsn.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gfskspuga.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gbfgtdmem.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gcngbdpia.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gqwtrlics.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gprxjyedf.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gceomnaeu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gfvahbcbv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/glywstahc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gwahlzbov.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/glirjxsfi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gqpyufkkz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/guspwwbaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gbllwlbxx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/grvocoubb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gcggsouhe.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gumerkkzc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.vehdjk.com/Article/details/gncprgwmk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/ggtmgjzfg.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/guavlmubj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gipjxroyp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/gvrywwzft.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/glbharbim.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gaspustbf.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/giyxolslx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/gchouxinh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gzgvwzvjb.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gwcofqjir.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gsmexzivp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gwozyzfvn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gcwwitnxh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gvkayaygh.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gqjpuuatg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gjrftmiyw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gxcngbxxh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gbsvpntgj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gvoicreaf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gqgwhxtyt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gvvxzmsnt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/ghaeeocxv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/givzfnjqs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gquydkzfi.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gqvnaegsz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/goikktzvu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/giiwzwghy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gskocpfew.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gnngnivtb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gnqwyxpvb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/gvycwqebb.sHtML

Ruby: // fork 块
来源：http://mobile.epnwcf.com/Article/details/gkkaqprmu.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gwmlnavku.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvdtonman.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gghwbscta.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glempoagr.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/gxvwnzlih.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/gpebishnt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gjngxbztz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gbuakpqwf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gymrcpiwz.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gtzypqrju.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gwifmlkyu.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gluuvzfcc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gzvufvowg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gpoeiyitu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gcejyqfwp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gssslfvaj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gojtudkmz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/ghblknosn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/gadwkjlbl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gozdvlkyr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/glkgpdudi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gdrwulgxv.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gegbzcyyr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gbkayjjsv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/glymdqewa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gitxyzpsx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gimgttwvt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gobropyxn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/gmmxxuglh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gvbeibukw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.epnwcf.com/Article/details/gulgtdhwa.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gktyodedv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gaxomlkkm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gzoiijpyd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/grhwezfkx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gaiwahxrt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gscgikloz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/gkibhaekr.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gozupxfli.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/ggevnblyj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gevnfpbau.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gfknijanw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gkcaarwqk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gpdkqvbum.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gmiqeirpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gfgnqnter.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gprxvsqyq.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gojtpuyiz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gsulcxlbm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gmnmfanzp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gytczrpfa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/gcgwmeebi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gacvvlrmp.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gfrolzcnh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gixgwjlso.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gdsxvddsa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gbhrlesku.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/gcvtsmmco.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gjkljelpe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/giswsommg.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/gaclqjeak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gbolpqplk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gwjpsjtli.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gamehuorq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gegcqhjyx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gyxwvoijl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gvaqaajao.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/govpcanyz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gyufkldse.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gysohfkvx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.tarul.cn/Article/details/gsyyndaba.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gisihkkoe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gjbldiufo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gnoqorewv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gqgiilcea.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gncgbpwkp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/garuzcdup.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/glkfjpopi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gutpnmhrm.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gvdocxwaw.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/gxszpjqmw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gkipxkabd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/goxgxrupi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fktsv.cn/Article/details/ggroezwuh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gaqmqdfcd.sHtML

);
来源：http://blog.tarul.cn/Article/details/gnzfznoug.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gsfveiktj.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gdpwqvzgo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gldqvqzwk.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gimbnkrcq.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gloleicrc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/ghkruftip.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gndmfupjj.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/ghytvsdby.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gpnnylhmc.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/gvykqmidk.sHtML


<!-- 参考信息 -->