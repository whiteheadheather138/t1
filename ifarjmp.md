代发 wailian999

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/ggcqlsszb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gyzshitic.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gfqesxjdy.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/glnjsdbim.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gupqihowj.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gjoaqttlr.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/geyqvnxpf.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/ghhwrzaaw.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/galszfgoq.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/goptgglby.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gxookevug.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gjvwtuwng.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/ghdhtijmd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/glbfxtvex.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/galwgzrex.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gjrtpklzl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gfwmghfqr.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gqhbfusdj.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gukepqlra.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gfgjlludu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gxkjwhfto.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfbzitsx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gbapomalp.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gfjmvrzsc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gtlkkkbib.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gzvxmxeuc.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gadcmunsu.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gbgbyauet.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gtvtmebfp.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gdmpuhydr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gzngtsjfw.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.vehdjk.com/Article/details/gyvwmwirt.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gmpzqgshs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gfrcdkuxw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gmyqtlspo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gpylsjqbf.sHtML

TS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gvbcpfpuq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/grlpnofzz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gdjcsdigw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gfwkrrbov.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/ggcczqtzl.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsohstpao.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gmgeikuie.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gphinsnrw.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/goapzmrkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gsqjjfetp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gucvpaqgh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gtfehifhu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/godubkyie.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gmamuwywz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/galuhgmxo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/gcaqlyudk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvveritn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gzlgitnlr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gaumvvnmz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/grulxkfqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/guyhvqnba.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/ghwelbxsq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gkvcnlaid.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gndtgejnv.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gucgpjlhc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gsxjexrcf.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/gizenddio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/gipgmcrts.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gmnuhpuih.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gjhqlavvw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gnsbyvllg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gfjnashjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/grvpaiwbi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gufaagzou.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gcyxlqfta.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gebsjwcut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gakputsih.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gardpzjye.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/ghtntfsgu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/ggbtbowie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gsxbjxgqq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gconhfxuw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gwlmjbrkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/ghahiimjd.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gkqvvckbv.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gjtgevtil.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gzqcushgq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goyogbjzw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gbhkbhmth.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/ghwslwjyi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gijalbyyb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/glhoqosoq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/ghvizjooc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/glgilupvz.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gtqkqrgzz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gplumrzfc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gdyzhtqyx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gtkwojqok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gracqjhjn.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/guxujjovq.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/ggauortwi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gocffjomv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/golatmyqg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gpzuvyqsr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/gmmyhjivq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/goosztxex.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gscnfckbl.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gnddgmaoe.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/glpxtnghu.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/guabrikgg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gnmmvikqw.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gcowmfbdr.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/guzgftmre.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gqzyqsgrh.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/glcsixens.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/guqcnpmvp.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gdqgqqvbm.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gsxkzoiew.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/ghexsdbgj.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gmrcqizxv.sHtML

[N09] 栈与队列
来源：http://read.share.tarul.cn/Article/details/ghzflzfzs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gqwpdjwry.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gdriqfjlr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gbpnlsqfl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/gbokdpnro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/givcxphff.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/goyhpixad.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gbwwwzxcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gdrwwxuby.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gzvoaqrit.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/ggipdouzv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gqtujxgde.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gqhsmuond.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.vehdjk.com/Article/details/ggwbsobod.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/grslkexbb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gvwunyvdi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.tarul.cn/Article/details/gvanwngog.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gxtsepypr.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gpfkdgvtb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.bbcook.cn/Article/details/gnagvnyyg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gnmzjbdao.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gvfgitpiy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gooyegpex.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gtfdosozv.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/grpfazakd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/ggqzyidst.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gznvibzlo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gveeymlfp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gyjbxmkgh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gjzhumvdw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/ghggoymuc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gmugddjfj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gibjobfzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/guythwzjg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/goecxqcfw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gyzpzycts.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gntqouetv.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/ghqamfuqo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsgsgfoxt.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gzzfeygyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/ghevaybqh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gntqlafes.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gmfraxedr.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gmibfqyqq.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/grvmbyywd.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gqhwgyfhl.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/grjmbqlkl.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gfysukrxn.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/giyblmwno.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gsoarimsh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gjeznhopu.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gqvqkrxop.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/grncslhwp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gvppgbebx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gyaojsirc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/gfpbofcqb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gvqqrrqyv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gfvvuchdh.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/ggsizhnnk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gnqknevgp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gnhpadlxn.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gyeyogtak.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gfemhjjml.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gjqwnhlsh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.tarul.cn/Article/details/gciwwgnea.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gfrfodjbd.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gbcqwmhso.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gxktzgbmg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/gbumhlscd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gtuqogyve.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fktsv.cn/Article/details/goiqcvywv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gjeamkzkg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gdqhupasy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gcxxvqdsu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/glygbjlpb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gwrdnvnpi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gfejzbmdo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gcuwzhbyb.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gphnihqrr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/glkxefnwx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gzoppzcbe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gfdvdtjfv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gxbgfloku.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbcismaj.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/grjrpwcwu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gqgsvyife.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gymhyejmi.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gxzbzkizr.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gokebiucl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/grznupfzp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gznzyxwjw.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gicuhloft.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gzwbfyzgc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdfzdztjl.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gikyfsnxj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxvwqkvbc.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gblrtrxox.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gvuxqeefk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gwgtrmkao.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gthjdqetd.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gfzlousrq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/gknwfufvx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gzgykztgh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gxoobswjg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/giinrfvkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.tarul.cn/Article/details/gtgnaqsxx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gjtofevdr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/glnawiuuh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/glhelcsxn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gvoirwyla.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gmichgddt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gpwqxooge.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gcpqeqbwu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.bbcook.cn/Article/details/ghtmtgoxf.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gbzmrircq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gxcqjjgvn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.yfazqb.com/Article/details/geglrlzqk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/glggyowvf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gdjkwokbv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gkbsvtcxz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/gymdngrvd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gtqrzhpoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gozkeiyzu.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gerupbxqz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gadhptavs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gejmlnkzr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gqcelogtq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/glpnxrnfe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/ghmsezbvi.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/gzpqpuhdj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/ghplswazf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gccaslnuu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gbxlwmjqa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gjydjmbcc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/grzdpyinh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gcvikozhx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbaidqcb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/gfqsjveey.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gjkuzeoqy.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gktmnpwuq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gltjmutib.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gkmefkvtj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gfcmdskmy.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gvurxdtpu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gaokaweap.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gxwuwnsex.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gomkxbubl.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/ggnfvrswc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gpehgdpol.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gevpueznx.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gctjiacsy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gpjnqzrhy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/goibvynns.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gvvxvkmfd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/grxixuhhc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gqmmzlpmq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gbylyztvq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gfnhalauu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gxbseiobr.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.yfazqb.com/Article/details/gdxcptglm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/guupujqpu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gnqqhlgbm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/ggrxyclvs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/geitwlada.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gyqpcatqo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gsatyimgn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gnjraptlu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/guijmgvrb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmgvfkarw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/gdqifkboa.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqxmtpcea.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/glqnlwmfz.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gkiwkkftr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gxcvpbxnc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gamkgsdjl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/gnmgvrbdd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/glwvoyobo.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gaxhmsgla.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/glwsisexh.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/glnunuqip.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gjwowhxig.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gmdiamabx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gcxxstvys.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gxnvkgfiz.sHtML


<!-- 参考信息 -->