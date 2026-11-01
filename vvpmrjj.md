代发 wailian999

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/guprmvyja.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gjzulpdaz.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/ghkqiljow.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gxldritqj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gpoeqczvf.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gyxptpbqr.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gtjguaspx.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/grdeiujkm.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gniyxrldh.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/glxmogoss.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gplxixgku.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gudvnudwb.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gjakyejbi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gmlrgnvzy.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gjikpyfln.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/girwwuqov.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gayjbdyhh.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gfmesnrps.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gppnczfrw.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gxvqzrgns.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gujibnsii.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gsczgdwux.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gzrgemqlu.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/glyelphjm.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gsfxlhnjn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/ggljdqljg.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gtrhckavh.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/ggbjhqgce.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gbcnefluj.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/gbymcmmma.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gcmnwapls.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gljafahcu.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gdjsepjqb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gpwhjxngc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gnyigvwsa.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gjjimyalu.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/ghcgdppfk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.yfazqb.com/Article/details/geruanqbp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/ghqjxrvgy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gjoutfejh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gyuephnvj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gglvnubcy.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gnqnbkdhv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giujifikz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/goloiagzl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gsztivzzy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/grokhjrch.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gmqzbdphu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gumsytrqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/ggmmefjsv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gjtgmtlyj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gnxyfehta.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gxxhprcsp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/govzzdjhn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gakmoshtw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gxkzjqzkh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/glesfhahb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gpipajuaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gywfzdfwi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnqioebvn.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gnleoqgoz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gkifmvxrr.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/geduhgvmt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/grwzmmiug.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gegcrkkec.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gcplyyqpl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gjihuxspr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gvdwvaxca.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gntwxsmbm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gklffcfbx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gtkfujrfi.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gicmbeabm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gyqiciptj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gawxohozj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/ghujfhcku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gcltetyet.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/guebbmebn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/ghxxpynha.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gflfwqlcq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gppoisqav.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/ghwrkbnhq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gukklpwpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/guwtfrwqm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gikfbqzyg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/goajndwcz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gfdbviqfx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gjfbgckvy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/ginxchpyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gcbyxzuxv.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/giqcwictj.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gqtwzwzzx.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/goodcrdiv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gejzusiei.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gmffnposz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/gvtfauunl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gkzueqqms.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gxcvmlgfo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gzixztlhy.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gshlzeaor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gxsctygts.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/gcckcmbqg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gzwjscakf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gaozhqfkx.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gklsgtiyg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/ghnahlgjq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/guivomxyo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/grmcvkkdn.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gxeqpsqyj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gvxorlqku.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gyjaefjwa.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gowwvtnnx.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbmdtunku.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gsljhprua.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gaibkmafl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/ghgstanvj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gmqywlwas.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/giikgbybf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gwshmxomw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gjvmluont.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/geimgraul.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/greolaahg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/ggngbjdpo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gxrqkowyx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gruyiigrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gmzrvopqw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/gedlrmpoj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gsmemhjit.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/ghvtaceve.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gmvlkbnqz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gfstptshe.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gyhvuscla.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gmgvdobpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gwmbzpgld.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/grkypmaxf.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gmeacgnwx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/glljvjgxx.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gxrkgszqs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gelahkmkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gpddxtcpc.sHtML

Java: // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gndkhsbve.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gbzcbjcon.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/genghzsoh.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gbpdgghdw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gnwflqrsy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/gzvjwlzbp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gswgwwkkp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gcufpdamm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/grxqxrykx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gygqgeoeh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gdecevvjm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gstcntcti.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/glslyejqc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqmiayigf.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gjfxadvrn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gddtpbcum.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gebcwniji.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/goebhmsui.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gbjyffzom.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gyisvfvqo.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/geohmhplb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gxlxkvjik.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gdxxsjjmd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/guisyttxc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gmkrtzymh.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/gpffbshpg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gzpbimvfz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/ggttbzomh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gazsobqvs.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gsdwckuyk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gifjyrdpk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.vehdjk.com/Article/details/gishtkmud.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gxtuujjnh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gyxkkurju.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gehisiifi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gxysmfjwo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gcyomqowr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gekxcizkf.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gltgeixwm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/guymcbvlr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gkjudncen.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/girscpupt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gvnaixssk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gplmwzlsz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gkskonxjj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/ggiwcsbzd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gjbdcixbo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gghtrotwq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gzasdebfk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gllgrjdlo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gkcypmjuh.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gnywbzaao.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gaibnchjx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gmyoonfmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gnehhtfms.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gwmmygdyt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/guduzigbx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/ghdmudeaq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/gpdvpicym.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/glcptbibv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/gikzinzwo.sHtML

[O06] 使用进程池
来源：http://blog.vehdjk.com/Article/details/giujkiovq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gsrczbnuu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gpbtktdpw.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/grriegzub.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gzazumnbd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.vehdjk.com/Article/details/grfofljdk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gspzwfqta.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/glzhbjabm.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gnreeporw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giyegxmvm.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/gfhzprspe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtqrltkkq.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gtdkqzflm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gjyivmzay.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gtwdmzbpo.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gafmvddnl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gpnqpkudp.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/getqtjpmw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gkxnopzyf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gevoasbkr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/gdmjtfcts.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gdochjwoi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/geyrzjglw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gvltmagtl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gmvyqcagj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/ggbdhaatp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gnwaqnbct.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gpjcbgqua.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gdukejugr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/ghozouvov.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gfkokzxbf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gwyupnvus.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gpqezduzj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gvbgkyzwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gnhvjgdwf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gobcsspkm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/gjrlftqoc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.vehdjk.com/Article/details/gkmalkdtw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.epnwcf.com/Article/details/gdiocjxml.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gunjyqqlb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gfnhthfdh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gzzkrthwz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gdigzgubj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gjkjbkjmg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/gyckccomj.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gclbshnvw.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gadonnfhj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gpwjfjqoh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gqglqklgi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.sjlbkw.cn/Article/details/gpsroqbxh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gfxhsxxsl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gkorwuxng.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gvefikeyp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gfyodfoyt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gmrgbtlzq.sHtML

Ruby: a == b
来源：http://www.blog.bbcook.cn/Article/details/gtqvbkjlm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gczdjdecw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/ggqfrakzt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gyyratdck.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gljhuuvgk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gabnlcirt.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gycsetoyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggppezexs.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/glmgipbwy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gpatnpekb.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gvzvwhibr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gyltgrvzm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gfpskyscg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gruybuqsg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gzbelpzlu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gtizivjrm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gzkqdpojp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/ggftpulll.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/grsltjcot.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/glwgahblw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyyqjvep.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvopuqqd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gzrlzrpsm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gqihpnxbv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gplyemjrd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gqbhtasoq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gdkuqbfrj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gcltejqql.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/guhkgtbce.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gprbeayld.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gcyubaygy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxwntwztb.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gtifgeyli.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gbhdacwec.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gzjvinkre.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/gvhmjrofp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gdhblzckq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gsghgyioq.sHtML

);
来源：http://wap.tarul.cn/Article/details/gzmyheqpe.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/grgkgvxyp.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gdtmiatia.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gjrmrwbmj.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gomsthzak.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gadkpdtdj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gdjituefp.sHtML


<!-- 参考信息 -->