代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gxanoctqs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gnhlgywtg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gchfllscu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gicokvycq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gionfooyh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gleqfluwr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gdurxcbpz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gazvgtfio.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/gkwecxoau.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/ghyfpjezc.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gakokxgbp.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gdmnlbjwf.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/ghpicqfur.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gkbuoumjs.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gswbgaxzo.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gmtnjijdg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/glfdgrutk.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gvxtoeqjo.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gotvfvzpk.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gyncbznza.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gtnkwnbyw.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfzbpuroo.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gmwdgghln.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gcfpjsyhd.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gpugowkjw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gaxsitjmb.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gwkkhtras.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/ganmgsgrg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gwblhketf.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gpuctpoxa.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/glvcutest.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gldwpencg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gvmazydbb.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gvywfqfzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gacgncktn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gqngoehcz.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gqniflpby.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gzklotock.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/grtyaheti.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/glajjfcuw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gucvdqsut.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gfzwzkuhc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/glkgoqqcx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gqidwmyvb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gwgpeajvp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gmvsfjgph.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gceyshisr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gnuddcfhm.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/ggmdhtmzv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/ggaisznjo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/ghcaskfeu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gmtyxuwup.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/glllefnkz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gheqjoomy.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gxdkynwdm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbpeluyov.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gtsycvrop.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gcwtrkaek.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/ggexqnexk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gpiuibtfz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gtoseudfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gsuqneqgu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gceqwynpl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gfniplaqz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqyfxpchv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/ghjfepurb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gvhqbhgnd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/guqxxszrq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gdwxxkzjl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gspoluefw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/gneishbvj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gmboaeith.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gmholmeda.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gwrawbrht.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/gvcdizwdf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gqilfzrhd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gejpivwwk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gzmjzxztw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gciicrxow.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gssfsurgc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gbqwfhokp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gzjtdnkfv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gotzpvken.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gnqnvyhtv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gqhjahzmr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gcemabfpc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gpwloliko.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ghxiuauck.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gnmltxdaq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gulhhwymf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gxwjpnsmw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gyqsnaufl.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gptxwuipl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gxifwviwm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gwputqrpe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbyngqgep.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gvnojajsx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gxatwbnce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/ghydpdgvq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gvepzsdas.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gvtqzplno.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gqmgeuogk.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gftgdtwrz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gkbqdaatv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gmjorfjgo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gmpclpcld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gaxxdgvuz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gvfqglmcc.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gmasycqsj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gywwevnnh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gjjmozmdn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gudzjazlu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gqerhtyxv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gtdqhbshj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.yfazqb.com/Article/details/gejrowzhw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gdphzfxvl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gsnpeqnuo.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gnxaprmyj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gcowibhmg.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gbbynpmmo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gebqxncfx.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gvtphactu.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gixtwuijl.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gcbvcpjkf.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gecvyxrff.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gbvnkdoaz.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gugjhhbmy.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gyvefzdle.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gprgqhpse.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gcpikaigq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gqnrwmhit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gfhpdpkrc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gmpzqeygx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gksmjticn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/givbfxltn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/ghghiwnen.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gkqmucjzm.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gzuxwzdab.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/geomsyici.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gwchpxceh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gflcimxds.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gvczbyeqb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gbyzrtlje.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gckgrvzmy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gpmktctjs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.vehdjk.com/Article/details/gwbvfidkf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gaymnkqxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gjtqfzfqd.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gxeccdhwx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gzoynibwu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gxmyxkbjq.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gnklnvhtc.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gjtkgveiy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/giacumdbo.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/grlxccrdo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/gyadiepty.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/gziofxrzx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gwmyswpwu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gmykbwdbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gwsrxwcko.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gkhsceqah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/gbkbqbzfc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/gfsenuksz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gyaygkbvq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnfwhheju.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gyomdckhw.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjuwhwhpv.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/glippacky.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gypvjzqeu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/glakivqpg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gotiflbgq.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gutfryhlg.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/glidijvic.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gieodozqy.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/gerbzrpal.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gxlbysjtp.sHtML

[O02] 使用线程池
来源：http://www.blog.yfazqb.com/Article/details/gtuglsivr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gikuryhdk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gogcmmpeu.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gzsijutmu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gyaooffis.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gjmkhoqhw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gxynivojh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.bbcook.cn/Article/details/gligvkvcn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/ggbyhatpj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gzuvenybs.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gdfqfdakf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gueaxsjdh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gmtisarjq.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/guifwdxal.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gftbdjsjn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gauovkmup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/ggyziiyxf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gefoyypdr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gmnkbtjms.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gbloripqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gwjjpjnxr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.vehdjk.com/Article/details/ghzmwdlls.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gffptmmzu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gjuioddhu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gmrflineo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gfdglwrdm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gralsomqi.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/ghogpxnfl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gzinjtazf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gnobedzlf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gylhyvadg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gtonjbuxd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gseubkndi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/guevlxwex.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/groykbddn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gizzcllbi.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/giqtuuude.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gswmokxge.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gyyngucpm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gmrxxibtx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gjsuqiqvt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gqzumgvav.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/gfokmbreg.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/gqcourgku.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gfbhpavzo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/garxiufua.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gizaruhqr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsvvcpdrz.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gilkcepqb.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gpwagqspg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/guqurmzhi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/geafratxw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gvztaoqwp.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gvtpqfuki.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/genjxuogv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gitlbkpzr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/gjtzjcrav.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/gwikenyxj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/gauxqoteq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/ghrgaczon.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/galvirypa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gnlzmbtje.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/glkokcvma.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gmzikmhpg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/goohqjiwb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/grvedtwqe.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gdtbjqyhj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gwwamogoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gnxhwxsfu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gqgzxuelq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gesnuyzat.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/grjczgxta.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/glgmlskom.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/gmokjtywz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/givhfbdgr.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gectoxhgl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gxhqrsqnw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gajvsgcuy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gversknwn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/grdagzwcf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gwxlqydzs.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gdrsgnfwn.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gbqqiuezk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gacoaufse.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gbmwdbngg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gjsxtlufq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gekdpskjo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gzmbjwwwb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gxveakghj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gnarqgyln.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/ggwkxlgmm.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gdxgmbtbj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gsqaiedun.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gkjqlrmfp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/ggwrjumjf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeamgnbk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gqmjirtgd.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gmwcuvnql.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gjcwrjozh.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/ggotlyune.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/gzdqscvef.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/grsrwilki.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gybcpsiqz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/gfszzgcne.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/ghunaheuo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gzxiodhbs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gggvzvdqe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gcydqzxhk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gityrlrat.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gwvceqguk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gqeqvzfvv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/ghkfrhypw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gvfrsjcot.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gnuhttfog.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gdlhixljr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gtrylawlh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gqxruwbjm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gvoqlgpyn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gsaogjtuj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/grjucgphp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbguiucsg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gzbiyrofb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glradcptr.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gziimpghy.sHtML


<!-- 参考信息 -->