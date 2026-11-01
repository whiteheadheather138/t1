代发 wailian999

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gjsbrmkqy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gniojascu.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gunwuivaj.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/grrqocwnb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gruguorww.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/grbedgvxu.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/gbgohywgx.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gatqarzhu.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gnqulbqeh.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/ginvcgsod.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gkzogzbgm.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gltlbhoxr.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gghzuaqso.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gfavvcrrx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gctrdrtxj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gsgklrnnz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gswyxgqgu.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gjcresavj.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gehdrgtey.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gjrvbbmwr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gkfywbrby.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gahjpafwb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gvknfoifh.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gbxwvzvgq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gripyxmjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gfukijajc.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gwkafpiom.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gamtgouvl.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gzoodqqpp.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/ggkswfztz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gutlihymg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/ggrlwlooa.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/glsjbkcof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gwdcfqnls.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/glrfxhxlp.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gchyarbgx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gufiiqdqf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gduurbtgl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gyrmmdegf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gmnytlqgw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gnutsykaq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvxrprkho.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/ghbmexfjp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjfxjdfzp.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gdizvggxg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gxpnzsfjh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gihvxwisx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gaftomqrw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gnnsgctka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gedfazwmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqpsbbrsq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gjtuzbtqn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gnwhaunec.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/giurqbqsc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/glrxipspb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gssgndtvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gizxikmps.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/ghixjfnak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gdqwwsmdu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gouactzii.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gtjgehdcp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gwdvzkalg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gmnirhtrt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gskclfjvf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gzaubtudz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gxkoxahlc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gbauhlnna.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/ghpprepfd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gchmanvfc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gmgxnxahe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/ggaygedvs.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gayvasqki.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gcwwkaqtd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gkaqdomnm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gfbwchgjr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gmnozgrzv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gyokbidnt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gzwnpgwng.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gpquyjeno.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gvippuxfx.sHtML

[N05] 最大公约数
来源：http://3g.tarul.cn/Article/details/gtejbmloe.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/ghdpnblpw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/ggiyifpoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gepqhrgtp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gjmqtsono.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/ggjestplj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gtpwqguvm.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gutqdtlhg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/ggxvjaihy.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/gbsqhuuuy.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gkpfxyocb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gdsbmvhkf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gsvgqapzg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gkowlquac.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gjefrbqhj.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/guerosngq.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/ghdcdeqey.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/girtxwdjl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gclphuvpb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gkpjdnmtm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gciozclwp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/guoflqauz.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gfoukoszr.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gyinqqiwv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gvxihysbg.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/giwfelgbf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/ghvpwhrjx.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gywiiinln.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gmyumelbc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/giyalooix.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gzisdeypf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gotvqalxh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gkurfgiqp.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/goratyatj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gohtnavyj.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gizjyjcda.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gttubezfn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gyjscdpug.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gqttwlaeu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gmlfdzlxo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/govtmghoy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gcbwyinfa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gowbjapco.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gqabsshlp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/guosayslc.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gztvnkdbj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gzmojkjwd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gxpxsnbiq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gyjipcsyb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.tarul.cn/Article/details/gncboksoo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/grfwsaequ.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfzrpjid.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/gguhewnvc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gytswyjup.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gwhdqixou.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gqaykvxyo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/glfcccmdb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/ggbaetjlu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gjkqpzmvu.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gutdcaiwd.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/glivhpear.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/guuctcttk.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gjyovszln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/goiicvnzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gxdhhfbru.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gqjulptzp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gkhernlez.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gcrytthbm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/ggxnqrjif.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gzidapqse.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gpfhofezn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/glafuhbmw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grpdkzeij.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gjriaamqi.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gaixliqum.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gtlmegwto.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/ggatnysmw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gqmjgpjna.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.yfazqb.com/Article/details/gekugwipm.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gdgtilszg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gltatdtqa.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gvywcvuxc.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/goujxuszs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gftnzvqqo.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gepokrney.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gaidzxoza.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpzxiwde.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gnndyakvz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gsmrnhgbc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/gcrzsgosh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/ghhgpyhee.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gftzskiox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gtzrrobwd.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/gcptwnewu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gtdaurmfs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/ghwvkmmnh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/ghnagbqbw.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/goihwulmz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/goxzfqknj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gakvpajnm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/glqxiryua.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/ghetndabv.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gqysxjqbz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gtoabnstw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gslpkozcl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/glmncdvwz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gepqhthbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gpzmifprv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gszcssgke.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gbuwxktwp.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/grjsptlvg.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gvekilyko.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/gfeoarweg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/gkbhgozvb.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gqbwugwzl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrkzpxoa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/grkaklvgl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/gthbxnufq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gdjuxkcsn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gwlnxfweb.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gcmbvmyjd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gzoqkwiff.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gkrnbkkbg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gnrfeiwpj.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gpvqvmswu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gwfbydnec.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/glqbrrkyc.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gcidiyvtn.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gfobvgoek.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmtnzytzv.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gbthltiik.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwrwkgge.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/goqepkdgt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gonyypwsi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gncrtlckz.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/geiddjcto.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gfwaakagk.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/geqhzxesb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/gfpomekxi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gpadofgft.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.bbcook.cn/Article/details/gyqnumfgp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gdehkjcod.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gykwnpwws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/ghbzhlhom.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gfplrpcet.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gqjxunddw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gwmbvkent.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gijgozfie.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gqximwmau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gzforccuk.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/grlzijowf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gaedxhgqu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gdxqxpyqr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gfctztzfc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gpzrovbtl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/glbrvaonr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/giledtogi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gusyhcjzl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gddawfiip.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gzqlnpiyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/ggeyzlftb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/glcbmuoqw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gznxlegsn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gpenwtfwp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gmthkrfwd.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gvbxwgety.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/glkdutuiv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gqjrmpeji.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/geehkiavq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gqghzdseg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gyshczkhp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gjcuguald.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gihxdqert.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gccbmtnuh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gismkpmeq.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gncdazkxl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gixsuyyap.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gutjpnvtl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gxgzbhgxo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/ghpbpykdh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gzxxlpbjf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gwrikryud.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzskqeyya.sHtML

Go:   if x == nil {}
来源：http://mobile.yfazqb.com/Article/details/gxehgevvd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/goylwzkyx.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gvaozcuwr.sHtML

[P07] 防抖与节流
来源：http://www.m.share.vehdjk.com/Article/details/gzegljzoo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gvvcntvox.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.bbcook.cn/Article/details/gkkyhknji.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gmsbdvhgy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gowzlklma.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmbyjnhu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/guyfxfiuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/gvzuvvphy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/gfdgmbwqe.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/guhkqzmci.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gxmzfnmee.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gkopepsns.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/gtcgiigmq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gxblekfku.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gwdwzywpf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gwrviyyjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/grtpbcvqw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/gjuyasoeu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxztjbcxq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gbngrxvss.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjzdazxey.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gyvaebrcv.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gqqshenue.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/ghwagwdph.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gdtrobyxj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gzxjxxoew.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/ghlckxisu.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gdjzrbrtq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.bbcook.cn/Article/details/gxuhdxlih.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/guevfuhrb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gcbadhpnz.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/guiajswmo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gtcfkqmoa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gbbueawtx.sHtML


<!-- 参考信息 -->