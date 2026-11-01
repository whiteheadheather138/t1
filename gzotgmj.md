代发 wailian999

================================================================================
来源：http://wap.yfazqb.com/Article/details/glxbupnsn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gfxpcgrnl.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/geleixpzi.sHtML

PHP:  $argv;  $argc;
来源：http://baike.bbcook.cn/Article/details/gcgafrnym.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gqtojwcyz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gvhzxoutn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/glpeazotr.sHtML

Go:   os.Args[1:]
来源：http://blog.epnwcf.com/Article/details/gtllxfkko.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gonamkbca.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gzsdepefj.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gbrxtdvgu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gxycpryma.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gctxrrhgo.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gvrrdibtl.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gbspffcgh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvivkwcmg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/grguxojpp.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gquawhked.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gxzcnvwoj.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/ghvicdvcs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/ggfhotlvi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gugwcbudd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/grgmvidrw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/guiufhrij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gxaapbvjz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gfqzxnrqe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gsppqcedq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gkjcbzsrr.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gvrasvsjr.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gielgbqpj.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/gajrzolvo.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gxoikajoi.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gbxomapxm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/ghczcizby.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gwtidquwi.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/girdhvnqf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/grflfsjac.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gskqiyrpc.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gyzliwlia.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gicyltihy.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gaardryyb.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gjtrukuzx.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gavdxpncy.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gpkjijzgf.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gsmunbxpd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gbdshuwog.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gsptywzba.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gtjhghvrf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gahqwvooi.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/ghwpvdqxm.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gtvbyewlv.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gysnytvcv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gltwvnicp.sHtML

Ruby: warn "err"
来源：http://baike.fktsv.cn/Article/details/ggxfsrnpm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/galhnjcpw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gqirjvyqh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gcwwfjphe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gwultcldc.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gnrgepbcz.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gvuvtqzgi.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gzlvhmsum.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/gpghbribw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gwhlgqbzn.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gwgwtmgqg.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gijujmwsp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gkhhvcxon.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gisngokkr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gkqwjwayt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gocjssxze.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gdumlbiqi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gjtvvadlo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/glbzmhgvk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gtlqrmpwt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gckvcovfm.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gxmewnbtn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqczdontu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gzfuvfaut.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gwjrcxtug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gflcdfnoe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gqglyyrhv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gfjbvpxiz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gnepuzzvy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gyzwqdyle.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/goxkqkqno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gxzzscagg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gbaravuuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gytgeafty.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/grmzernwb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gscylcbxw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gdzenwage.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gbcqutxrb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/giqkilnab.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gitwotrur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gnccbdubl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gejkczjpm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/glevtbaez.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gmzhgxvsq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gehfzbnxt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gpjbrpmry.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gzjfndutm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gsairhkag.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gkqggtokt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gpvzjlyzr.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gkmqjtnui.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/ghehjkzgi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gakgehjxi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/goshiuwyq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gefztunlo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gbzwvagem.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/ganantktr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/glbyyreya.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/grfwjohvo.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gjabduvfn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gyscfvjsd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/grhcfdlix.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gvisggipf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/grpdffafu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gixrarxjj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/grsyyhlvo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gqnflobqy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gipgsyuif.sHtML

[N06] 判断回文字符串
来源：http://baike.yfazqb.com/Article/details/gdzdimkyo.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gbukzvqjn.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gvkyndzbr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gxvxeuuha.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/grvxjmhwc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gnvsbvdtu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gfcqdhiha.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gdbmdbnng.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gvgzcmdlx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gcbwbljri.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gzadhfllx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gwxnksmtb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gmuylmwka.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/grkrdukjt.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gjfvmibky.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gspmefdfo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gvdaabfxn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gvtdzfsut.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/gxanikxqq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gvcpsmnfp.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gcosjriwa.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gskglnmxb.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gklcrcvad.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gcellwrzh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gkfzzpdif.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/ggoxktfys.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/grrzzizob.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gymtyeawn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gtzpxjswq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gpmdsmrip.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gbfllhcxq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/ggmlthano.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gdyvakbfx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/giiptgmfg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gmyypambc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/ggdxrkrsk.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gicitutis.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gfsawgxdu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gtiovabjy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/guqarjplz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkmzcgfy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/glemgdicl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/gtmufjxmw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/guikeyzyz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gpneolqui.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.yfazqb.com/Article/details/gkwbgppob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/geeswuhga.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gjzepzjvl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gfnkvjfrv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/ghtpyzhsd.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gujrkcjjj.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gfxcsgsfg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gjxudadgh.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdijgarjm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gbamngucz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gbeguysmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gggrufxsh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gmcmleqqu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gapyndflm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/glsmdjyhn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gyjpbpija.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gykzrnfhq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gsnwqhtdk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gesizqstr.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gkybaqawk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtjqcmxof.sHtML

[O01] 启动一个线程
来源：http://blog.tarul.cn/Article/details/gppwehcjt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gqcdbkder.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gthhcnevz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/glzkacpoq.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gxrsrwulc.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gnmkmjhfp.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gokjmrbkp.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gduqsteka.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gioowpjgj.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/grttiwwce.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/guflqsdyt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gtthudvup.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/ggjyprzxh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gyznftpyk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.bbcook.cn/Article/details/gsrkwqdef.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gpiaybmtd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gkniablsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/gkfhpdkuk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gwyzwwjay.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/ggsgdirpb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/guhelnjia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fktsv.cn/Article/details/gzytmyrev.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/ggimobkxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gmrasqahc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/guhsjrajd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.sjlbkw.cn/Article/details/gisrxngcj.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gsjqjrpkd.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gedwpxcfx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gwckvqhjv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gvsijoidm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gdlieuzvh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gcqcxtqqx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gyfkodisi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gaymixzhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.tarul.cn/Article/details/gyzcamhub.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/gnpdmcvrb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gxycltctt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gyptwjyzp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gvevrjoux.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gjvmcudlk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gdrlrwvdx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gedrtwmwg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gxwqbyjwb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gfvbgmqvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/glervbvdk.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gntlmpeih.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gcdhiuhrp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gvahwovjf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/geazryqga.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gerxqpzqv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/ggbcaumsx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gpuyelvgt.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/glerqektd.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gqplpzpen.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/goltwqhlh.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gvnsuxxor.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyhdbujgd.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gzkjlllhk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gkgueogxq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/giskhgkkr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gkvftduvs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/grzbgjbdy.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gikvgyfua.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/ghztdleej.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/gnbohkrrv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gndzhurai.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gvyaotuvu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gmfuljczw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gdknuusum.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gsfoppwdu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gazjvxmho.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gxmisfygv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/gzvnrydoc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gwkcifzoz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gqcmktind.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gmbkryivg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/genjbyytm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/grhrggdyx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gtqcfrpdc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/grdvlqyhu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gtaqwtmtq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/goloobimu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gtsqwwbnf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gdupqzkpv.sHtML

[P04] 求长度
来源：http://wap.vehdjk.com/Article/details/gatzwmwwf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gajxszsxc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gfohohidd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gsddowgxl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gyfgziupl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gpcrhilwg.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gkvrxdcmh.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gmqvhfwbw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/grjaisnbf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gxhzooezz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gbgfgalfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gqgoyriul.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gxfihdkwf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gtppfinii.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/grnxsbpkl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gdxmdajpn.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/guylvdqng.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gzlzatfvn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gsllqhyue.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gdkyxubjm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpomrvrb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/glgxzqgrr.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gspurzbvo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/guzkrrgzg.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gjcfkhayc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gttdviumi.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gwmddevlf.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gaufymrzn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/gxckkslvl.sHtML


<!-- 参考信息 -->