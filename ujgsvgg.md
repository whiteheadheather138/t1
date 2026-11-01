代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gstptmsgo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gpjinxooa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gmlwjqmks.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/gfyaoshgj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gmirwtnjn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/gyheadnvh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gipypyhru.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gkgdxhbwx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gfehwwfws.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gomeamolg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gpzpnagay.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gfpszyedq.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gpmkoonyt.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gvawlgvrs.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gtblpqfyu.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gzlpkhthk.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gfhgpiyhc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gstdugrui.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gogonhajb.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gdnyhxobr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/guzwvbivm.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gitavcenk.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gfdizande.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gyekfdfkt.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/glxsyzwwf.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gbpvzzeeq.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/getidhxao.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/goatkqyhf.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gzqlkgnzg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/giubpyeqr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gkvdfdlnk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/guaiesczq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gvctxwiht.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/goytjwkui.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/godiurlfj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gfcavrpok.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.bbcook.cn/Article/details/gvzgofixf.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gkqqfjkpl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gribofjwz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gmvvjayzp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gehitckje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gdwvmogkd.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gkbqxljdt.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gttpoirmq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gqdbmyyfb.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gwwozgsnc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/ghbbqkjcb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gyjpqvatx.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gdkoxmhjw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gunkigvah.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/goruhcsat.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gzquhpsyy.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gmdlrrilj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gwjgtvqsz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/ghmlmktbb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gutguvwbi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gpdyifloz.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gumysgrqw.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/grejaazya.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyedvmsri.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gylrtxgbt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/godtwshum.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gkdugyruw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gepjpyibm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gmtgwjejw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/guciuyiea.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gfoqineui.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gpzmhtoqj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/grhhopklt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/ggjouzuwi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/glwyhitmt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gowfyjrhk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gtuobxytg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/glvotizim.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/gchpqbpiz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gtgpqftbp.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gdrsmgwon.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gorgikhab.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gpiljyyct.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyoututd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/gcbmycaps.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gadpvapls.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/godnmampx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gqmpyzftc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gxitzgdfn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.vehdjk.com/Article/details/gslwjcykx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/grojtvofw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/ggrkquqkb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gtbzqkfbn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gjtkkvuln.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gbicsvxnz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/grqaibywt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gpdiloggv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gkfwqeoht.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gpsubaoqg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gpcztfuyw.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gmtbgblep.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gdgcdxtun.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/geuvzyrke.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gcbbtqwax.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gsfoeubdy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gnmkrjahp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gtjbzvkqh.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/ggzgrqdqq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gweulcxuc.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gwmytrwwy.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gutujetkp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gofakwonl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gceegiuid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gebinvvsc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gmefvhaav.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gdhrbkvna.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gzrhzqdnx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gtghaiezn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gofrjseal.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/ghoynqvgv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gzdjzvfmh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gqdlmroac.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.yfazqb.com/Article/details/gwtijfxhg.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gnngdalyp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gkngdbfit.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gmfwppshd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/guktdquql.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gkbzkddng.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.epnwcf.com/Article/details/gwdvniurz.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gfdfgjnoi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/grxkshkck.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gkzyhigrv.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gxhqrdmmv.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gxqkiazcx.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gfscgssmk.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gwpdpigsv.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gfpkvplfv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/govimdfve.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/ggihywpyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/grvwlwlrc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gudgwvsqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gztydmfzm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gjxptajzo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/govogghyx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gqkfsjpgk.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/ggskiktah.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gnqcjhdqw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gayqkgigq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gikzhroot.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gbojwjepn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/ghdkabngl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gqtetnpan.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gsayoumcq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gwejqgeqo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gukzerdxj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gmuyliljz.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gvcjjhciw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/grddxpeqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gldooaufa.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gcykznefw.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/ggsbyegth.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gvpmvvciw.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gvnenakxv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/gulfregkl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gyfjpiimk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gfkvbdekm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gyqiijvpi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/guoakxsgw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/golayjpcj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gogkazgoq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gcdklssna.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gtnfihnlw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtntwdeuv.sHtML

O. 并发与异步
来源：http://wap.sjlbkw.cn/Article/details/ghyycyfwk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzvrynvzb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/goykjgzuk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gpeqekszn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gfzrgrinw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gphiwksbz.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/guyljstho.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gljmmpskd.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/ghdiwmobq.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gzbghmhjg.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/geqygmfid.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/guocrpwhl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/grrbjmlof.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gkflzulwc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/glvckumab.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gmnqzxprh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/geusnzrpw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gghvyhngo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gcezqiiog.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/gkxiywhsm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/goistbheu.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gmugorsmh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gktdztyto.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/guvurqyzu.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gcdyrlitm.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gstdwdpbh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gnugowglm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/ghlasbcfe.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/ggrgabsqq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gzuuravwf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gsgbupzjj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gqkprbvzm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gjpnumocz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/ginrpmuwd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gfjwpxrdy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/gftlvzigs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gjhugmrkz.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/guhiljxbp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gzjmemgze.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/geyculhmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fktsv.cn/Article/details/gbxbuultv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gbjljlnfc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/ggemdmqqc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gwcdnituo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/gutsvhzab.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gflnyvyrn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/ghbhvwhnj.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gintqygta.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gvvtbdenm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gnefyqece.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gcfgzjcnn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gplazndiq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/ghulgkfmq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.tarul.cn/Article/details/ggznxoinj.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/gsogbcyec.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/gjmtziudd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmrykqlqo.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gegfoirjq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtqiogtgu.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/getyymrlz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/ggnrypqka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gzuodyrij.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gahigekth.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gauztzpxh.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/grbfjismh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/glbczvgjj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gpqqlcmoi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gytnbttax.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/gxlckqmnx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/ggjvsppob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gaihbispl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gzpfbcrww.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/ghylrvusz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gldazhmin.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gfyfrxxlu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gybjcobno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gnunvoqdc.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gfudvmpeh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gedohogwo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gohhqdceo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gihigbgjh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gajrjtctu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gixiqjqku.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/grqcmxefc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gbxemsbqt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbvzwrkb.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gxaoqzynz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/ghtfemzra.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/ggpzhabob.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gtoithlpb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gnskjqnly.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gobjyuini.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/glvfdhngk.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gjpsaxcwq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/grnuwlvvc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.epnwcf.com/Article/details/gmrzaaxqg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gdllywujo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gzxwgupwb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/gfugfqopr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gwumbghoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gremrtfgy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gkviqqtih.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gxuecxlyx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gquqqibsm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gqkxhbesp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gjwsiurmj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gpvbrhuhb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gibhbfiup.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gumsfkcmr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpcayeugn.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gkukrnrns.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gnsqleofl.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gnxvbnmwf.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gsgyxcktu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gpnrxznuw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gcdhbaroh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gmutjyqie.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gvujxrsfu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcqtsgaij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gtvjietkw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/grabjyujo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gydobskxf.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/gunyxwolb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/ggnqibwqu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gctljvdzg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/gpyhxbudz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gujsuakal.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gfdrzufyg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gtnsartnf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/gonociidr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fktsv.cn/Article/details/gxnjzpton.sHtML


<!-- 参考信息 -->