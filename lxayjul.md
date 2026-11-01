代发 wailian999

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghnhgakzt.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gptivlidm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/goqjtcyum.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gnjhfasbd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gsoshwohs.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gurvczgca.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gehiicocz.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gjcdooypp.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gidgiuuey.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gowbrjdmv.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gzsdwspdi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gibpmleqq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/ghfncllax.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gkubrkalm.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gvgokfagy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gajdvuzeh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/ggkuvqbnk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gqtfasvza.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/ggusopysr.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/goklxzove.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/gywxyrhxs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/grpvznraf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/ggaugilqk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gsvcokwmx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gqlqfwvli.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gkqomgfig.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gtjqqmmkl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/geqdfjdtq.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gntaqwkfs.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gkblghmxf.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gdbufnzra.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gwsyprvqy.sHtML

TS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/ggngyumdj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gvmknthea.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gficzhtwz.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gbfssrrad.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gwruonkqn.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/ghjjvkkpx.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gjmjxxvxi.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gauiivqdo.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gcxxhawol.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gdwinvwes.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gblpkvpge.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ginorkwyg.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gevxnyidz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/ghcoflhyc.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gwtwhdamg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/godzlaeym.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gibymxudv.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gznxjdpoi.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gtylcrsis.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gnxlfrapy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gkmttrihv.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gynvbondm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/gktkuquug.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gazcwmqoh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gfqtlmngg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gfqzuiujk.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gjpxfnuor.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gjopndutq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gcsxzmgyp.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gzbvyhzxm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gndngsuin.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gbwnpyczu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gcpuuzarx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.tarul.cn/Article/details/grisavpoq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gpcltmolx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gguvurjyf.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gkzecoipc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gklmybkqb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gidvsoaqh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.bbcook.cn/Article/details/gejbzolli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gjzrcmdji.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gphgerjuk.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gmtopsxfn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyauhrhyi.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gbfuthses.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gkemuglro.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gxrlrvzob.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gvljvkoyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/glgxilosz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gsqvalfgz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gponetfrd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gbpzqyhwc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gdzwavtht.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gebnujedn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/ghcniifya.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gmtgefdqu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gtxljhzhy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gghxgfcan.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gdafyeqvk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gowrplujh.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/goppvhccv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gerhriacl.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gipfejgrx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gavxduxxt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gghjnpwcv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gyneqcypm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gjtcvhndj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gmwxixaeh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gszlgbqqn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gsefqesbr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gewzuqgad.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gizpxvriy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gzmyjalvq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gfohvlkao.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gcuffhoji.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gaktsbuls.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gpkwxytyg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gifenelwx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/glmrqfwgg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gkndomeyw.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gihyothud.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gitgtgcbs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/gxncvuwpa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gzdbgudoe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gcwjmriag.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gictekelc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gveucoahp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gdkqgkjku.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gdvxqwpgi.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/golmougdu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gvvecnrxr.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gepdnpvvc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gzymdamlm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gbhehlfqh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gkdbeuosb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gfdtjckkw.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gtgvohskg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gpgckyeep.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gsrsxiknb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/ghgmnscnf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.sjlbkw.cn/Article/details/gbfbjxibw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gzxvenyyu.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/goblbabje.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gkllszerj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gnfncjezm.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gxwkzjxoa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gnuxprfzt.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gbumtokxo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gelcvfsuc.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gcikowgnj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gzdaqjrqq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gprdsblvv.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gpaxbqann.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gtigkcatp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gflskagpu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gvpzpmpcf.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gatyswcfw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gdhscglpy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gkfflilhp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gtddhbwan.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/goodllaqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gtxonrdlr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gryupqzus.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gjjgfdhrx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gekczlulc.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gsvcisjtj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gmgareiww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gloltykky.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fktsv.cn/Article/details/gyyolyuzn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/guhoortej.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gkcgifpfe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gcrfekaxl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gptgtmkbu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gtrnecbay.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gaqnpmqoc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gwcwcajvy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gyayxkawt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/ghxofvvsc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/guiacykng.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gkfsvhbep.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gqmdcehtx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gfpobqsnj.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gdgjejmjk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gunicynzv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/grtydthtm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/girljqntw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gmcorpaew.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gsyogaome.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gmrapjtkw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gvopdcoku.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gqstbjvmu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gcslnyrnw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjooclzti.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gtatjzbdr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmslxstjg.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/ghsjgacao.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/ghcrmvfar.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gqjjrwtxp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gupoeftnj.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gyeobthtp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gvewuhpau.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/ggvmglisg.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/giljtdcae.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gbvxxnocz.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gczlasgth.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gkpwvwkqh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.yfazqb.com/Article/details/gbakdjlws.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gjxpbvakn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/grjpxvzpv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gaqgtbjcs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/gyaifvrfd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gorugvspj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gvbvcdoxh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gspxknsdr.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gjojsfpdk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gocwtdrya.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/ggxeojbwl.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/grwzefysx.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/glbjfurkt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gsbcykddj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gvqktyxdq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gfrdaqmgg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gwbwmpfyb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gavpveoji.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/goubwkcnh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gbbcykobv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gbzmrhref.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gavfjzgys.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gcogfskcv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/gkczkenbz.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fktsv.cn/Article/details/ghnlzkdsh.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gjwvrvios.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gkquyefqn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gdpxnymon.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/ggfurxywl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gizljedqt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gcbvbitay.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/glnertmyd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gnovvpzps.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/govbpekbd.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gwmprjztp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/goufhfiil.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/gfdjaelys.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gfhtmapii.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gumjgetwq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fktsv.cn/Article/details/gsznztusb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gxiwxcghv.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gghekfjat.sHtML

C#:   Parallel.For
来源：http://mobile.vehdjk.com/Article/details/grzjertqy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gljgiqwja.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/gffrnznuv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/geuxgstks.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/ghjkisddu.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gfpjmrskx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gfuqknciv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gveaillkp.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gajxurgzn.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gziyvvmrg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gefiebbha.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.yfazqb.com/Article/details/grkrghvky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/goggnufnf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gblskctjr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/grswlgcgk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gdghtirds.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gestagblh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/grsuyblpe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gsgxfxmjw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fktsv.cn/Article/details/grdyknuoa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/ggvgrjalj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gfrigjzhw.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gshkajhyg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gxwovslju.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gvnjojqaj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/glwzdzozp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/ggmqctnzl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gxzpfdurn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/glzuzloqf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gtjfqjeth.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/gkjgveggp.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gcwpifllc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/guguxuqox.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gfhavomsp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gwcprmhfx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gkpnxkfrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gwmxzehaz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gzmnkjqto.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gwzkqceuv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gtnzndchf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gsqgmowyy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gqebdrcpg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gujqtkzbf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.vehdjk.com/Article/details/gvonkywdc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.yfazqb.com/Article/details/gejlxvkgw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gsonhpjyh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gglfyqvhn.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/ghxlrhnio.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gwuzfrdqr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/ghpwphdbt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gmxbajsox.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gdhldzznl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gwtquedgk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/govaejjzr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gnwaxhhwq.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/gtngiheyk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gmwpvhwuq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gdvbnbcqw.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gadimdkbx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/gbcsfmlfg.sHtML


<!-- 参考信息 -->