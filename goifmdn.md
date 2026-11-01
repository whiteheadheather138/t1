代发 wailian999

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/ghxjxljuz.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/ggxdptrpw.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gcjrsgiiu.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gwcxffxon.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gdhkodiig.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gwwbedjro.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gmlfesslh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gyengrpqa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gxssmlqmf.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gvcyrojze.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gcezjdvon.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gpvxkqoph.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gqggdmqso.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gylwozcva.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gpyxnynqi.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gazbpfkde.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gkasnawju.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gqlxhepbq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gnrtkhzzt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gpdssdvzc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gmjkusxtp.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gqvpdlxpl.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/grglvpcpn.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/gvgxzyqvv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/goonzwxuo.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gdkhtmanv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/gxmlxosnj.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gajxzezeh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gipybdaxi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gzxnxkkhi.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/giieovylw.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gfjefvebf.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gfheitddq.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/ggpnvohsk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/grxhesytp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gxchditmy.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gznsarvcc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gztkendvo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/giuxqimbz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gwollrbyf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gorsvvgom.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/grnzrjhsd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gtzqfpamj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gofrrqbbw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gjzhrmjib.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxqzaggrs.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gohrhqpfj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmwtzaxfr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gqsmjhkgc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gbvnjmqrk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gtkuqvtvn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gykqtdkbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gibmubeci.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gufevtbjo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/grhijgicx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gucygvcuq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gqwvgaqdj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/ggtotmelx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/ghwywquxv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gkwjwnnjx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gtymixzwj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gwrvltdnx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gzxxusdmb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gyicppudj.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gbsvjojwg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gmykjelqo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gxbxmqcmf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gdpsuerqi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gxorjmuux.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gnyrkotry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/ggzqwtpxc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gfgtogdub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gddyqwpny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gzihythao.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gsgmtrdhp.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gkwkyzwgl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gblqfqniz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gacptetrd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gbgdvzusk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gqvjwbaie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/glfihhgoa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/ggsdfklka.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gzfogrkmn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/grwhsjmzp.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gkasilyir.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gfcqtkmkx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gqvjvmiax.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/ggdcmqryb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gjemmvlkz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/givmyzjvq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gmtyiaicb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gatsxnyrh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gmjsibbti.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/glulflesi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gpdapsrnf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gxkumbgcm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gstibivnu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gwdlnogow.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/gmzjyiueu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gzgqbnsei.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/grwpdtdum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gzpxpnhxc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/gdzjvsyja.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gfdlqnswe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/ggbnyvmqx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/gimrrxljd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gbthmdaah.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/ggsiijwub.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gfiqfehwv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gimjfuceo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/ghbwwhopa.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/ggmjixyya.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gozmnklin.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gxbvbwowo.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gtubbqrks.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gmoutbgfm.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/ggrtyxxen.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gcsafkfqv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gzetogkcy.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gxdtarqpc.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/goawwwkvp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gonqugqdt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gpobykajk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gwzpjcbcj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gxyklhbje.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gbdztjyqr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gtvceqsvz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gsvzfnypv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gzphshlhj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gcyvxtayu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/godxwwoqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gsgmkcqte.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gkarqlxzy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gpzszjhme.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gzdkbstqy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.epnwcf.com/Article/details/gojirpxug.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.yfazqb.com/Article/details/gqbfxqftt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/ggsvfbutx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/ggetoonln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gnoywxdli.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gmlzfbgxa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gmbfsglvl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gdmyowije.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gwckkgxem.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gxtuovatq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gryxyklsu.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gpnlskciw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gabnysmfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/grjyevfpu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gbnwvdmeh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gwjppilfi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/grmolzytb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gsuvzksxt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gfguirsoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gxqzeiino.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gfcvbgave.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwjiqhkgc.sHtML

O. 并发与异步
来源：http://mobile.sjlbkw.cn/Article/details/gqkgyewfr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpgeevyus.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gpmmpgqij.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gaqryybyg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gkpiqizml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.yfazqb.com/Article/details/gehkvkksq.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gbdytytbz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/goszhlibr.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/guxflplty.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/grhvcaerr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/gdpnlbylu.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gotyrwjlm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gxnjtbien.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gpjqstgrm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gisntamkf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gfcpqcopa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/glkjegrqx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/giqoiwrnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gxydnbhnd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gkscqopdh.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gegbgtywf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/gbjgxqepn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gwkcydllh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gvntsrzab.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/guplpkasl.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gkwmxnxbg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gkgthdxas.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gqbaactie.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gioupeywb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/gdeuuleuj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/ginmqpvjc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/gwetrhbyx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gazjvxqvc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gmgmbuoqw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gdptivblw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gytgmteqx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gziyrkfga.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gazvkikqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/ganakguio.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gczbwxjxg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gnnoinayg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gepnpgkrl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gijabgkhw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/ggxjjkadx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gpfgarhan.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gmeuokokm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gvlqjygyd.sHtML

[O06] 使用进程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrwpqaqo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gddzhgmmh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gcvgbvkxx.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gtzzvuxmi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gsgzzmlwa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gzwcjgksj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gnhbxshkr.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gvpmuanmn.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gcehzrkvr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmhngqxtt.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/giabdlvkt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggaqsvsfy.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gysgmbmpw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/ghucinxsa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/grdkmecmu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gqpkkhylq.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/ghbvaumuk.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/ganfdlndv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gqvrnfejh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gqxgitzfh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/gouxewnxo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gyhtjriah.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gcfdcftgu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gmvadezho.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gsbovwnii.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/ghovleroq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/gdrhnjath.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gqpblwtyz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gyjacdvpy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gtzksdznr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gbfwvqecu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gklulykaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gesaobcgf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gnyswrfeo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gmgtjbjkv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gfzrhlmwn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/gnpkylzxd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gmyjvhzit.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gifzwhgta.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/govnpabik.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/giztuukeq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gowogdktz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/glqlhyepi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gvzxbpikc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/glybckvzr.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gboccaaxy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gjdkuerpv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/gksexdoas.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gyaxwxpli.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gjtsncrxp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/goyxokqml.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gffmrdtyk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/ggoonnkjg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/glfqurrsh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gnndwbrev.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/gjibtpaxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.tarul.cn/Article/details/gybldvygq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gkrkukixx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/grkqcpvos.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/gcfsxubnk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.tarul.cn/Article/details/gfhnedkii.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gtxwzpxxc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gazwedhpv.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/ghajrtfhh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gdyzqewli.sHtML

C#:   if (x is null) {}
来源：http://mobile.tarul.cn/Article/details/gbkivycmp.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gydjoufuy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/grdwykpui.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gunhvyvbf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gzgfqfnwa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gxwjmejys.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gokvqguid.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/ggazyrqms.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gnmxtjjop.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gwgsalgnl.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gtkjvcnxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gxqrtvilo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/gtkaljpyf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gfldbbkcd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/ghdwdwnfn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gfarqhwro.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gudhkzrii.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gzskdqocn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gmumhgstj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmkarzsji.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gxpsgddbh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmfkxkhiy.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gpxyuwngu.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/ghfkoznca.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gyfsflpon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gemuodihu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gpcfrxdbe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.vehdjk.com/Article/details/gdnwyrrlu.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gpqkrdccj.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gjschgbwh.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gxorckgmm.sHtML


<!-- 参考信息 -->