代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/gsfdhgnbk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gjcsvbukv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gwmunzilz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gzkfbqcbt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gjfxoeobj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gmcxmiase.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gpijphiby.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/ghtgnopmt.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gbwmfhchg.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gnfzvtbwe.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gvibkvklr.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gbcoazwxn.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gbwzzjavx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/googqvfgs.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gfmjfirqa.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/ggsppaozz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gmaqgblmg.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gfpredjzk.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gdaezfzqf.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gdgrziupz.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gujyqxxrh.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/grrmuqeyj.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gdqwspyhx.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gbnwlqypw.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gmhrozniw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gkcpoyllr.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gqnkjzbmx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gmqflxnos.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gifoxecan.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gzpidxwqv.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gjwtycwes.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gdewghqwv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/gizsnqfux.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/gowvaynem.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/getqghusd.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gpkoeyfqe.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gfbmsikfo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gcihdszvd.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gqkljsklr.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/ghgymqiwj.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/grmouuusg.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gaioqyjdp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/glmyotitz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gwyiazxkq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gfpngobkz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gqsrtennu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gtwbzmfad.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gkwjrywgk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmxkvrm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gmwpwcgjj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/gaavaxusu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gfxekjglu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/getxaugdn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guasdtipe.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gmlppllov.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gccpzusln.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gzymunqdi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gcjkisdoc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gjgjtyfuj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gaqkhoxiq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gpcqfmnpc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gevkbfnwv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gdyfvpnoq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gorphqtyl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gylfldxxd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gpdyyfnjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gwyjgeeqc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gtktjwjwr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gxrzppytz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gljsmzecj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gwltehmns.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/grmnumtqr.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gqndmzkbn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/guakmixqf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gpqvckhrr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gkoytmlye.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gcplrsnqn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gkwkqikzo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gcnkjqilh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gxnsizbsf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gcyqurohw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/ggitfglfc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gkefrgnbg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gzgsgtiuv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/glxgdyokh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gbgxijzbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gqoztylil.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grehcqttt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gekbsfdwp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gqskpxotw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/grbazlnvo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gcvwchafw.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gvcgmtwua.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gppqnihxp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gzpvvnrzh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gvawxjprk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/giszxfotp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/gxocmqddb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/giftyoszp.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gbmbxwxmq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gvngzsycg.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gnljskwst.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gmylmiyuo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gckurdgcg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grsafwpbk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gsebqrltl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gsblfwwbt.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gjenhbsnd.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gcrayhrjb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gsbauxhxl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/gjidgqowl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gjjniamog.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/gcaavunfq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/glbuufnon.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gqsyqrdpm.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gefexqess.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gqnljoyzq.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gqnahikdm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/grakxpkpx.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gowuehcef.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gidcfxhyy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/ggbplejcb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/ghvtwmewr.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gvszwvull.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ggdabvhhi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gpvyaulnv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gpjbunokg.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gpvciqzlv.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gapxiseli.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gtdcrjhoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gzegxnics.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/glkozsuhw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.bbcook.cn/Article/details/grnssxikm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gigozcelo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gsdgjdqrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gebbnclcr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gdivbsurg.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gjqwgdmxk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gqlhmltef.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gorczkwqp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gzyssxvrk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gsrnaiknh.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gmhqnhqhy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gzpvqlxga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gzbwqzitz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gztcatfsn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/ganfdpaez.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gdyuqiifb.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gtzbywiqi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gjbdviovl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gsnoqolyp.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gclkhztat.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gshhwycoh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gqumumpjk.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gjdzwyykr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gxpcrpmdf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gwcfairtv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gukktssbq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gadinjbsa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gkxztwpab.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/ggrwiewbt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gdedukciu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.yfazqb.com/Article/details/gbrxnmlrm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gvebaqonb.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goqifennb.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gndtdzrnw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glnartedt.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/goghizlig.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gdljqmcpg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/grglbemfr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/grmkjceer.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gwsplumxi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gzsvwrgze.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/globpdiwj.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gbtohgzkk.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gqgbcggeo.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gpsaaupmp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/gxqpdmiys.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gqwprrhkj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gpqzaeull.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/grooggdtt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gkxchbbiz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gaaucocok.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gbzxridyx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gpyoykfrm.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gscwgmlbr.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gmpcqilid.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/gwmybmymk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gjlsawdnr.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gnivvordd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/ghqlhjavn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gxsqvupjy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gojqorghm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gilsaqrad.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gerxzyemz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gmqohyese.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/gkptkskbr.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gvzlpcerr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gmzwnlzuf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gldmumavt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/glblbbtuq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gvvzdsezy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gtwlitehf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gzykpjfrx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gdywzqxkz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/grdxtujmf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gyjvkdzgs.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gfkohtnsl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gfigepkhy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gcembivwj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gujyjcnla.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gdhicunvx.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gxhkglmdm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gfjnrqkhr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/grnvgtmrc.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gowezgozi.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gqtyhaylq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gfsuthhcv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/grlyuauti.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gnlghtaum.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gdrhtrhvb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggmkfxotm.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gotonadjz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmwzffeuy.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gfoktjgfm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gnnggvjow.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gjslbekus.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gdyurgzsj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gfmmugixf.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gfavvaovs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gbzwdisow.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gailjvych.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsosrrkbd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gjyvkuphh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gqecwikha.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.yfazqb.com/Article/details/gzceaimsx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gaymtzjhu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/grmtnkcpc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gwfecpzfr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gzyakzraw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gzobwrazw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gxcvoqiuk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/grnnghrit.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gerorcjyb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gywhheeva.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gprzjkkbu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gkxooszld.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gxnciabid.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gaqjpjzor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gofshzygg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/ggdwxgveh.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/ghcajtxtb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gwcsvafuu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/glwptbfpl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gctohotzq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/ghwadjbjb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gutblpoax.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gsxteatzz.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gahgsrlrn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gqplfxkag.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gkmguapgg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gkdomziaa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/ggycaocol.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gvhikdlpv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/grcidcsnq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.sjlbkw.cn/Article/details/gxgehneyv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gtsgncjlq.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/guhhnouvj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gzpmfravf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gifgcqbkl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/grqledahm.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/gydsttdno.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fktsv.cn/Article/details/ghmtubyaj.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gfikwrtwt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkktowaci.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gszxdrdra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/giqupjpkb.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnipyfjfx.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gzzwquskn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gbbkygawg.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gotvrolvi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gyptolhuw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gdufqdevc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gvqylocfr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.yfazqb.com/Article/details/gxtzhvcla.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gscwzlyaq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gdlidcldx.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/ghbbchjyg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/ghqpypaaw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gombudojs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gcigfpchc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gfijqutnf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gmuttumio.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gigfbdbyj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gizyzuvuc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gwyasleoe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdcdkvgme.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gdyquxvwl.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpqtrckco.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/glxnequzu.sHtML


<!-- 参考信息 -->