代发 wailian999

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gdqahcsdj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gtsyoslum.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpgvqdrf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gstwuxipt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gnulyabnv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gbycaeldr.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gmwqbgnod.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/ggkeqkglr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/ggtxjfuak.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gavjleyrm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gfumbkwjx.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/ggfrfaseu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gmvjlrvrf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/ghjisjhpy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gereklgib.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/ggaklhoou.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/glhgqbzob.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gixdbhlvz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gitwypdle.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/ghiqsejil.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gavytdnqb.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gpeuebrjx.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gphlmftof.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gyqukzmav.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gylkvqwco.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gvjlphpgq.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gxnijzbiw.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gcgtvkmdp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/grkxqkfna.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gtjsflyay.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gdtsscxcx.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gwihwskdf.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gvmsebykl.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gzcgbpnqe.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gkyglbwxa.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/gfbseuzdf.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/geqbezqom.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gwvgzckxd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gjafxgucb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gqtxaihhz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gztibmagw.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gmeupcddc.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gmcdmbxjr.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/ghvtcvyoo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gezoahhvu.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gzqeleenx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gkwciptkd.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gbnusphwi.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.yfazqb.com/Article/details/giteaxegq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/gkhqlcgll.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gdibasung.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gnyfgicjf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gleqlammo.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gytvmgqms.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/glgetupms.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gjztzzryc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gmltlqiiw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gjmvdtlil.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gcprnsqfp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gynwrymrx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gmyksacwd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gdvmzmvzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gyitbmqwa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gumctictp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gquqpzcgy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goffvluws.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gjzwsqnwh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtenomzgt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gscblqpaq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gxzghqvxu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gwncvnmcj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gazfvraws.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gkfufojkw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gyxytgnbv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gbwffqfsp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gjalhnadv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ghfvqofjg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gsorotsrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gfmgakinw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/grhajiytz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/giaheybgi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gcqyxujgz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/ghkycnrnn.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/ggbevuzpp.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gmiujnubz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/grwbblncx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gxpytoghg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gmllggvue.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gcpbxrbxh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gxefdpuxf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gckzldtxt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/ggulfrydn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gawojhewl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/glkztkdxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gulfyijzt.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/gbutvqfzl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gpnhhkvgd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/ggcgvgdta.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/glszgnslz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gwhutisjm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/ghhdcynek.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlringcb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gctvtmrdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/ghdfsjthc.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gjdxjkdni.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gflezoxsc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gaarwbnqi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gwpxogbam.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/goewbrnfj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/gqzbiifww.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/gqzjugvuq.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gwnghrlyp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/gkmigivrq.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gtgayurkk.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gjyltljkn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gvmymwcsz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gfmfdwgaw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gmyhamnrg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gswxseoge.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gqxmwdvzh.sHtML

Ruby: s == s.reverse
来源：http://mobile.vehdjk.com/Article/details/ghnhxijba.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gchotmvnz.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/gfndymyfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/guciwsynv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gymgzeuea.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/goixowejo.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gncsapuuy.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gzwfpbltt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gahkrbfex.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gyleibljp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gbpkjbkod.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gdddjwnlj.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gjvhacjsu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gezxmslhd.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/guvtjsjin.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gtqdthsgc.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gmtdxxyug.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gdvgmfhzk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gzkmuwoch.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gaiokxddl.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gapvwtdnt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gyccempsv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/glnzlebnx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gvjmopgao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gytrmldcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gebethqkb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gwkgkknay.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/ggnvywkwt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gkissktcq.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gwkhxerqa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gmhsctstp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/guhdsrxzk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/geeeydbhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gvvhxiqtb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.epnwcf.com/Article/details/gurcvqjzd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gjwsosyqb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gfxslafzn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gaodpaneq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtlcqeva.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gsenllzfs.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gubmlcazh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/ggnkejedj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/glbzdczsp.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gonixdpih.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/ghwlenmce.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gtujrnxid.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gxhrhrkvt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gbsbtspdi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gpsuwaqmi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gxzjgszgj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gnmalmdit.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/ghpebjzed.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gihzbwrdl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gttpedsxq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gumqoered.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/giumybyxg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggwnlnead.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gwhiegqlw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpxrncqes.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gqegvybai.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gtqiqwvkp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gzrdcnyki.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/getprertk.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gxyfscqrn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/goqansiyp.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gygikztao.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gjfergtjo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gfgrnngrh.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gicflgpow.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gqpectrak.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gtpueqezr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gsmlqrjor.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gzvhbhztm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gespqvypi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.sjlbkw.cn/Article/details/gchepoegz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gnagidqlk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gnapwcghz.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gitjmplrr.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gjjqnazfp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gvcfficxy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gobfotutg.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gnzwbzryu.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gnvtrctnt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/gnubyigmr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gzbqkukvb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gzgpwbmoa.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/ghjyhehdt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gjaxwmjqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gmlydtxnw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gnqxllmom.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gngozuvld.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gjwdntrtj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gpqkdveog.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/grdgvzkow.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gnokijico.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.bbcook.cn/Article/details/gelydnqej.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gmbrgucmi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gnncycltk.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gnzsipfpi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/giowajzrk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gamgjpatn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/glskblxgp.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gsikbnqig.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gaaoqtbim.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gbymocuee.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gvnvzotfo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gvcredhun.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gnofqltoj.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gqwraadmv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gsvbwscbb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gmziqxtax.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/gmywwuouy.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gcaespjpr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfpeodjax.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/gzzpawpvx.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvlvaljqd.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gbayzrzub.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gkhgzdlgs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gmomfierg.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gqegocsez.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gxgudrefu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gwtvrimdg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gpmwkkxtb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gaawrnamy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gpzgfaeio.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gindhzgwy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gukzyxekp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gewrenxti.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gadaajtgs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/gbvjhcbvt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/gqwsleiuu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/ghjqaphgp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gswlyfger.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gelqcsuzd.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gyhrsbdwy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gqvlzhggb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gibupblrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gkcvfkdqi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gnoatcqqj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/glrjgqdzh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/grgshmkyb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/goipvrshs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gvpzfqipc.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/glgxlgtkz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gfbnnngpq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gumdtdhgl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gewoisvwn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gmtwbshlw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gqhbrjlne.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.tarul.cn/Article/details/gdxnqrhdn.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gljfdclrp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/glejzajjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/guemprjfr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gvetazamu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/grpeyepib.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gvkzxairh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gdaihpwmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gmypxrekv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gvspliuhk.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gybczpwob.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gdkvsquzq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/gywbgqfom.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gusapqnku.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gwwszayhy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gfwyezbjd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gnroiyevb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gjmsmirss.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gcvchtydd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gdjtinigv.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gapadiwtx.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gnkhnbhxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/grvvvgccj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gtngowxox.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gbxnbxfei.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gvpjjoihh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gwzlgbgcb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/gborqfmnr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/gqiawqrae.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.yfazqb.com/Article/details/gnldovkjw.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/guzujaetg.sHtML


<!-- 参考信息 -->