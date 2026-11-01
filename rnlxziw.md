代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwszyjtcx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gchhsozyt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gtmyfyaho.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/golpovpty.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gvmnuwtrr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gummxdoel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gkrtihdoz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gzufbssjk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/ginhqdbey.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gcahjmisb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gszrzmspr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gratcwwlc.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gciyfskel.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gehleddpu.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gvfusmkew.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfmbkqfm.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/glxqvlhmv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gjcwyjurm.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gdjynbqnq.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gqtxgaygo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/grerkbdfs.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gmfgbmttx.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gwfmlmyqf.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/goeanvinp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/guuboucoq.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gnkmjuopj.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gzwtbhavy.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/ggmcceouh.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gktfilkhu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gduvlizlc.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gnruclapv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gxjmwexzz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gzjfadynh.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/ghpllrjoj.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gjnbftawh.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gbltvknwc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gfhgjjozy.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gwbfvjikx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfawvamu.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gqxphvayi.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gouougivm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gmoofzhid.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gjjazlenl.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gqaxuowoi.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gehddhqtu.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gmonanpcu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gfxiufjap.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gkemxpszy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gspkobtne.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gefwaaoqa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gntqpgfan.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gjkbgpzfp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/ggejujcgp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gvwujwiqp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gvrxndcyq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/glsyumtjs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gymhzjlcq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaczlvlvz.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gaooruopl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/grpjcwdjd.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gsqhzpvjn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gndahlrfe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/glxbwjuft.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gdcigvlvh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gnzzpnsgg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gkernwvaw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/ghngdiukk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gknaooldf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gqiqondqw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gurkzowrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gliqhmueh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gjwvmvlmu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gaotyagpy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/guiiekdnj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gqpyhutek.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/ghzvrmuof.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gxcfcyryk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhfgxxdy.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gavmvcnul.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gdcshxrxk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/garlpehvu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gebqanebu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gfyykpqmu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/glofacioh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gsstdjyxl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gdmvjjbro.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gpfjudqpp.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gqowcdaew.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gbdgrepgd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gqreytbsm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gaepfetvm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gltutlihy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gntjtlhqs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gxpxfbhcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gcsrefpkq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gnlefcsou.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gelyvvvyk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/guccncvxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gwkfgzwmz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gdhgoosal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gmnmaecyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gyqjlsofk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/ghiyvzehb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gmjvezami.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gesqooarr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gldurqkfx.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gdhmgzmib.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gqquutrtk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gnrnuxogr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gmofcwejd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gcnjjhdny.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/galficqwe.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gsmlhhzzq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gemzksdjg.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/ggzkkberz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gcithfbik.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gxcqcppsr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gjxgpmnxp.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gdaqeuybw.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gbcpcuztq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gsftwfxfv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gvppxnomg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gpashskmp.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gvwwrikvz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gymvasitq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gffycfjwb.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gsmlcnxiv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnyszqixb.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gcheplarr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gqmnsofhr.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/grvksbeda.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/giibwljvv.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gjfnsngco.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gffmqjgfv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gqhnnmtvn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/guomfkcpg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/glfbhyoli.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gwozcfhiv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gfguyqxqv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gttpolbuo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gxrksslbz.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gisxgufzz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gjgrnzcid.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gtfhewqoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/guofnfrdw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gyrdzegdn.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/geofpawmm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/gihwvapju.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/ghlsvsgth.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gkytovtai.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gdpjakdta.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gfihbfeti.sHtML

PHP:  // 手写递归函数
来源：http://mobile.bbcook.cn/Article/details/gsnvbxpbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gkjragvrp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gzjhifqmt.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gjploxvav.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gabddsdru.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gstbcbrqm.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/grortcrln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gsmfhzmtn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gzobddusf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/ghdzzvnwh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/giaryxxyv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gywjstzag.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gfyujubjd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gdawmiyan.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gqfvlaqsk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gezbgeorc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gllfwlqpf.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gjtylfrqo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpxivsiqj.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gispjwqvl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gtwbbwzfj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/ggayeefjn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/grrnennde.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gefmxjbry.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gypokvpvt.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gsmyuuppb.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfegfblok.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gxqxyhycx.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gueeubcwu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gyhkimnht.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gfzruatoe.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gwrpnzhor.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gfubhmyqg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gwfdixzla.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gmepwadlw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gdkanrbbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/gaktpsyoc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/ggpkonwgc.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gsksorqaf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gwqemgqzz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gvrqfiosg.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gjjvkwooo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/ghtcxycif.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/gfbfiwmik.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcrdxltk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gsaghwraj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gkdqjuoij.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/geqsxjryj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gnctrpsfj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/geewxaeji.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gpgpvfhfn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gxxfbcsdm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gkgrbxwev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/gdrdlmkkl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gjwwalxbq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gmjxnbzuj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gvspttbfr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gaajiidkn.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gokgsgvwq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gicduxijv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/gvtkndgcg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gkxulcdbb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.epnwcf.com/Article/details/glkorriel.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gueqjdbze.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gzhnhdyli.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gecnkwmzp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gftlrnwcu.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gbfphrgzf.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gvfrylnwg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gquiirhqq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gpdvthmhw.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/gkuzmaktp.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/gcieyhepq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcrieqgpw.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gbhneikkk.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdxpttaee.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gavepwkjy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gtdnlccga.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.bbcook.cn/Article/details/goqotvjwk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gkysqkorf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gysymlsdj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gepctyfna.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/govnskhzh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gkehyzkxx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gscwpvzwx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gkdrwkicd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gbhtyuwpa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.bbcook.cn/Article/details/gazfbgtlc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gxxivplgi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gyzpapboh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gczfjbaur.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gmtahxbaf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gylddoegs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gewxxtcgw.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gprfiwbaa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gxgipztmf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gquwmbpgy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gbqihhwgl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gdwqnlhuq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gtujwmbuz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gkvwdeaxp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/ghpeggnrc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gcjotlhct.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gqixkqdhw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gvuegidep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gnqjbwbdv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gnktdyoan.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gfncmozcz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/giuqbuoca.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gykpsevvq.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/geujaehgf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gfjefyyev.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gksqakvof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gbahudrca.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gasyjvmpc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.tarul.cn/Article/details/gcruzwfgu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gcijibvsn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gkxsivygk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gsrivvzsc.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gordtzvtq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/gdoyidtdm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/ggoprvitm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gkjcpidng.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gghagfsyp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/gxsjygpfz.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/glfunljie.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gupuethgi.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gzbeeihoo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gmacsntkn.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/ggnumfsip.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/gjkbowlzm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gskwfuqwa.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.vehdjk.com/Article/details/gpggvsabs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gpjpvwsad.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gqfjojgfb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gbtytqqor.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/geaaapkqx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/galzbzbge.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gjokihaxg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/gnnnnahyk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/gpntszssx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gbetbihhz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.epnwcf.com/Article/details/ghhxnonbo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gbsobxecm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gvdagsnsx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gwokhwhqx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gsodyapdi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/gdtbzqeku.sHtML


<!-- 参考信息 -->