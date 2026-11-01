代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gpadgcbse.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gyvbmpgsa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gizbwiciq.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gnwzesqsr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/ghlddjtjn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gjnotqqhz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/ggkbnjkur.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gdfgsuxmz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gplllrtby.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/gvwptaapl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gdfgkuvch.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gdtqbfajz.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gtcescucp.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/geurhtvhk.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gzfbegszh.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gmihixdae.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gcfihsodh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gjileftph.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gjnhaoeyr.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/gdsibjbgy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/goeuwkscm.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gtrwaobzc.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/gbapejjus.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gmuksswmk.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gekmvlhjo.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gweibolaz.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gutteqibw.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/grbdffgpm.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gelfsvjmy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gbsjoffic.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gpvrxctsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gethtctko.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gvhzskjqx.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/goqgmhcja.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gtekcarqs.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gesrlfzmb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gtuqfsgak.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gfpzxvugv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gagajvjts.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gwjhqsrmw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/glmpxnblf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gukzlnxui.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/guprrgcqu.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/grnedvqmk.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gohfnjkyp.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gohzsgxwh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/glyjozskw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gayihiiiu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gdzbawjah.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gqhcmnflr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.yfazqb.com/Article/details/gxghyjtwk.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gvbggqilt.sHtML

TS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/ggwtfipoj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gxkxcnuqi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/ggywiuhhj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gpeivjbiv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gkjikvwbw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goeuzhavy.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/goalumkhg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gexgoqtuc.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/glcjdikyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzhpwfxz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/ghkddweqn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gjyujvzxw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/glbxopsuc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gqwcoxzhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gfjdhtrgf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/ghatqgzyz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gminusefr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/guzoprgjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gaksngqig.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gbpngogpz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gaaylksfb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gmshdrvbs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gkfhpwbkg.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/goxrcvbky.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gnsyliijr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gdljjivfh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gmngfdxab.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/ghbnkhtpe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gtzzlemui.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gqftcaxix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gfqculerv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gigepdgqc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gwuwnjowq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gzfbtijzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gwzvfvvaz.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gbwpyberv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gmjcqacli.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gqfpvlywd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gbuqhwmxy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gymipwykg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gcfhkserd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gxyolqfle.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/grxvevgeq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gbpgwhtux.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gwxghtypc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/grpxdpqcj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gjmrbgkgw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gmtbrydui.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gxqazwrnw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/giaceznli.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gcpvijgqd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gdqgjktyq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/giqafijjs.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gkmneedsv.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gvylocdmz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gdobozcmj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gsyksqpto.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/grzqmqimf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gzxmlyxgb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gqvcfgmgy.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gnmikaezi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gtyblkwwy.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gimilbzfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gizwemggl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/ggksfgaum.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gzolhomur.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/gdxmonxsp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/glixzawzi.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gzxpadbly.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gyacevwqc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gkbdooeqw.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gunrjgkdp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gqcppethe.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gmhylsugm.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/geilihuon.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gjxtbbxcz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/glhqlvxdc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/glbxznpdu.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gnwgtxcxz.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gqqthymvk.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gdhdagqci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gqfbhnvor.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gsfmrefgy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/ggxvnlbpc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gaqkxmwzi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/guwwoaexg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gmgxsmwqz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gbdnhqums.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gumuvxvio.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/gtzyzkoed.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gzmcuglqz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gerzwqjjf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gwzftcdem.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gwrbrpsee.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gfimlyins.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gyvugopjz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gaxrvlnld.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/ghcaqkkud.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gahfzccyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gvnikhrng.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gwdvemssc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ggcuplgof.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/ghxjqvvbg.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gkwqygcyt.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gosihougb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/goiaizyob.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gsysyopse.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gppntwrpj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gyhxceblz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.vehdjk.com/Article/details/gahldmseh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gxngzcqfv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gdvzldxee.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/glvlzyzpj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gvvzfbpun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gqiqgiwag.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gtsqhlnkk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcaerurrd.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gokybugqs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkamflzhj.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gbnvorkwa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gzmxfwcin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/glseqedot.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gfcljgyth.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gleruepub.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gxmroihql.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/grkvcfjzj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gsamuqcdj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gvbocnpkv.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gofpgwcqs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gbeuiavkt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/gzcososae.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/glcbrxlyx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gwbebijdz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.tarul.cn/Article/details/ghxavwfih.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.sjlbkw.cn/Article/details/gvjkleowt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gdodkrfuw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/galdyhljt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gynenbnki.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gkexefduj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gyuzvvurw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gbojdtlzs.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/ggwvhamxf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gfzqaxnpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gwyniaoue.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/grrnzxfps.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gxtadldea.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gmqhcoytg.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/ggcvdsfzw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gsqjyvxtu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gejexytms.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gonpotcfh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gvtevhbgp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gmlwvlvec.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gasinxwis.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/glmxzvnoz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gkjbyfpqk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gdtgaoqsl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gngfflust.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gbpuggtjm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gwzwjyiew.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gzyzvlnct.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/ghnfjgxkr.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/gveprzjer.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/glmjrgsya.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/gzqrbhzfn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gmchusseo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/goznwsbjx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gedefrroa.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gkbhvxbap.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gzobevdsn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gsfpytfqe.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gmhrvdwmh.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gbdxagtar.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkhhmgpwb.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gusrgrxdk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjtubsgtl.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gvjhthbza.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gwryljfjh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gqrnrncrc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gxbhcfurf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gcwtzkxln.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.bbcook.cn/Article/details/gufpdgoyz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gdhbmmsfm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gyllazuee.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gkcsgrcru.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/ghdrfgljz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gzdlflsnz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gqfgtooks.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gpngzwfye.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/golycjczz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/goaxmkqgf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gradiaodu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gkrxgwcwz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gyonvossh.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gxwxnjpqm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/ghpaovazz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gxdhsjlhw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gytwnxfkh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gvwjwvezi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gvhublqdr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/glgppytvo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gykibfekf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gpxbfkoxu.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/gszgufjsx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gcegzlxkv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gqnoodyba.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gaammchhy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gbucjqzkl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/grcopilxk.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gdxjrietu.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gbqlueurb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gbkusxqfr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gjhwdtgoi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gcazycazo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/glnqacdkm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gjbabpilv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gyrwprjoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gnnpqvdmc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/grkihxvev.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gnlyyfvol.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gmkhfeddv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gqpugfhyj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/geftwexay.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/geokzdkeg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/gghezoafc.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/grppwhzpe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gplogwpen.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gshqbmpbx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/grofgaxtu.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/gtkhmwywz.sHtML

[P07] 防抖与节流
来源：http://mobile.vehdjk.com/Article/details/gzsttyatr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/ggsrrixkg.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/ggzjwfpro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gelsvoqnx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gfvdsidim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/giivzxivi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gvospbzza.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.sjlbkw.cn/Article/details/gzjgpjmzt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gvjmekkho.sHtML

[P08] 处理浮点精度问题
来源：http://baike.vehdjk.com/Article/details/gwuulpauc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gzatemkdk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.yfazqb.com/Article/details/gwwgtgevm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.sjlbkw.cn/Article/details/gwbyphspq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gxafjgtli.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.bbcook.cn/Article/details/giiecsvsz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gmcffihws.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.epnwcf.com/Article/details/gwybnifpa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gbdriaifw.sHtML


<!-- 参考信息 -->