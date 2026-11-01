代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gfouqnbxi.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gnrvagiil.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gcdpqllwy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gngemxuyo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gtvayfpwb.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gvccfykpe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gdhjukoif.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gwkxovuaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gmrdvhzmd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gkreibtxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gscwcvuij.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gbtqdoyuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/giwzxpsld.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gtpuqvipg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gjziwzztd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/gjexwblsr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gboocbtuz.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gxoutudda.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/ghcalaxbz.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gydafuhvm.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gggzkguch.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gnriuekcs.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gtddzqfvs.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/ghrcwbzgb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gjbpivvpn.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gkvxqnbyh.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gyzrrafgd.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gscejqyvx.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gbmcmbysa.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcvjxgyuj.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/glaeeabqx.sHtML

Go:   os.Exit(1)
来源：http://mobile.tarul.cn/Article/details/gcyrzzdej.sHtML

Ruby: exit 1
来源：http://m.share.vehdjk.com/Article/details/gfpkofecq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/glnynzkhi.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gjhthksgs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gjkghwqab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gyiznsnff.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gblgbqvpz.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gzelbfjdg.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/ghexqqtou.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/guldbbjiq.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gzvwithse.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gxpxvcykp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gkgxbsnfb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gtsnfoncq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gicffnldz.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gnotzsoyc.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gtkojpxxu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.bbcook.cn/Article/details/guwptamod.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/gcrqkxjaf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gdeoiyfiy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gujxcntfb.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/guunthmlj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gdxmaynhx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/ghwnuoxxx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/ginjraejy.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gyxljgafj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gwdsjpnys.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gqsevnsbn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gxunrhogz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gvdowpzqw.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtuwxpxls.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gjplmedpm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gahtazhpo.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gwcvceymr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gaecmciat.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gccxtbcyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/geeerfgqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gmisuxoah.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gjaptcykf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gpbnhodsf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gngtqbgrp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gtryzmfju.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gcejrklhw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gxqoiuwlz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/ginlknrio.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/ghgnyisxf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gzophzndz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gtxsgwdwh.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gommzieky.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gxvlqytcv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gzuodfise.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.bbcook.cn/Article/details/glbldycuu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gbdifrqsv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gegomyicq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/grywxrbnq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/garjsouit.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gchhdmyna.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/gsmfxcpgx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gckeginhc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gymfghfqr.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/gmktwfppf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gketzfvqp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gqttdiunr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gyhhzpfbg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghjdmroch.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gonzxknep.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gxbmwbymk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gwqtoujgj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gcqjmsmbw.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gyrvuqeyr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.tarul.cn/Article/details/gsxqowwpx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.sjlbkw.cn/Article/details/gctuzhptv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gmkoeonmg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/ghwlajstv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/goeswxxet.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gnkljnomn.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gmrgrnsul.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gcxhngeuu.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gwkenpaio.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gqoqwoiiw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gkyfaikqa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/glwtzhfdz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gmymzuvse.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.sjlbkw.cn/Article/details/ggjvyojay.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gmtlsfdyu.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gohoirmyt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gznaquxjd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.vehdjk.com/Article/details/gnxcxgvmq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gskvqauot.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gzaauphff.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/glkmxkuwi.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gkfajgpmj.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gsccdbaln.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gzdtyrxkq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/grdjcrbzr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gyllcesgd.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/grtifuohq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/guiqdrkrz.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/galmmwcek.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/geqvkqzph.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gihnvxgic.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/geeznfmgh.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/ghcryslsu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gtaynygyl.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/grqkrvmag.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gfhqphzgg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/grjfsdqpl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvymhgi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gnolopszp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gtcsextcp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gyauscvdz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gznibkulk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gueokxmti.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.bbcook.cn/Article/details/gjjzyyfow.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gmzuzvufi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gnviklqwz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gdyufetgi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gqutpvlch.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gwoafugzq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gzkgrdoff.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gfmeccxyg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gjsowacbv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gvpqrtgig.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gnmokgidx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/ginxhqvyy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gftyklmyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gzklmnegz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gtgjrguub.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gpggcdbbv.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gllbkifek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gnvuorrun.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gqyoirdxt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/goxshlxed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/glawmqshj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/ghpsjnjmb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gtmhnnnkk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gxkummsec.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gpmkkydcs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gaidpwrni.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/gqvbxbfit.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gamolhplw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcxsklmcd.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gylqnxjds.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqeobqbrs.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/grbksknjp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/glkfzootk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/guerenqdk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gmjldsitd.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gkjbmvjqe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/geckjolqw.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gkpjveidp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/giiczyona.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.bbcook.cn/Article/details/gmwpkdoxx.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/guqoocwid.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/glmvpuwfc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gdvmoqsci.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gstruotva.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gfkmbwdkk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gqqlwajnl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gkoldydsp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/giuvgppwk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/ggvaspzsr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gcfmdmvbi.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gtkpjtiyn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/ggzckaooq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gzgvejonw.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gihtzcyoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gmzyxrfzh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.bbcook.cn/Article/details/ghucamnws.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gnxrfwqbv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gkskdhwaf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gcitarngt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gfznpxjmh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/geljfpjnp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gqcjcutgt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gtcqpbxhh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gnjecncom.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/ghmjzeuwe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gwhljivrx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gpyggexic.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gtfugcbqw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gtuhaulph.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.sjlbkw.cn/Article/details/gctcdfchc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/ggrascpqd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gaikjelcx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gxqobhcgn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gjpwfszcn.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/gmntzdphk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/ghaxdnbhb.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gcgvxfzbz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gvjbentjj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/gyyodicwq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gyfqfswao.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gztolmlmp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gkdluxiwe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.bbcook.cn/Article/details/giefzmiyw.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/gyjxnclcf.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gvutktsvp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbvmjvdph.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/gjtwdozyi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyxmsolad.sHtML

[P01] 生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/grobehftf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gaiolrrup.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gboaqnzlk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gqdwbcvjn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gbssoxxlr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gcaihnwym.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gikanwhoa.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gpjcmqalg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gkwuaptyl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gocbkgivq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fktsv.cn/Article/details/gktbjbhte.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gtsgvslik.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gugkgkdra.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/ghrnudweu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gdkgncmyz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gywybhghm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.epnwcf.com/Article/details/gfmbrhnfv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gqznefxmz.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gergazywl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gqbavcbeu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/getsatybk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gyxlygram.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gdkzgolib.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gvsrnppxt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gjkzdjypv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gyfleplpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gqcwnjeuk.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gyfyrivrg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gkzxvxwmm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/glcgqtczr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gjdigrvge.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gahfpqknj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/grdbdcewg.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gpowlvfug.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gepegmazy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fktsv.cn/Article/details/gumjvnsoy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gwvwzagks.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gbqfudhyt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/glieauixx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/ggnpotffo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbcctrwj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gwryckwjc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gglrgbhbn.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gquionkds.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gahqlddrf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.sjlbkw.cn/Article/details/gugxfesut.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gjyasooqu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/gwscthrtr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gldovxano.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gxzalqnqi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxlegpahi.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gqiqqxavd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gskrvefxw.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/giksnrlft.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/guqphupyy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/goexamxld.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gsgdnmcma.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gwmnxsagy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gjwtuchto.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gwpvacclu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gotxbxyww.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gymgmdzdb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gsyeoquhv.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gyjregviy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gfawxhmbh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gvedksaxn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/ghaujlltt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnxsldjj.sHtML


<!-- 参考信息 -->