代发 wailian999

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gldywhkoi.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gbxpddiwv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/goeqwrrso.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/giqfrowbq.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gcihhjzzu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gmdhlgsoy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gukxujpch.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gzgutcybm.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/guwgevyid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gaezxebys.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/grtglrdfu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/grjvsfevl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gfmxxfkso.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gabxzcaho.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gilufepan.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gdingiebz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.vehdjk.com/Article/details/geiqgtyzc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gltnkgjuz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gbbmiqbrq.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/grmatqrva.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gdarloziy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gqvqhcpii.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/ghbkxliwb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gspemsagi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gnjvfjrya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/gwifdopdf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gjaocnuuc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/gaxwftxeg.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gevgkihxq.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gmaxadzwn.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/godjsgkjq.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gqeohzoae.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gchqipggg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gyooniibl.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/gjtpideus.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gamoeyimy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/guywzjgaj.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gcqnewyum.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gzanfbrjx.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gxwexgpla.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/girhxmnkh.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzhrmbren.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gzkaskaaw.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gbsrkuuei.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gherxhwss.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gotkelmuw.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gsrmjtcjo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gjnhngtgq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gxnvuukew.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gzieuflql.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gkcauchvn.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gyjeoqgeq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gxkpvcfks.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gorgjjtpv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/ghdeefals.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gsexzanrh.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gyiqtkroq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gdxhhklyp.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gmvdeutav.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/ggifswxwp.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gfuhjoxrv.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gspsnectp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gjdrjznhc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gdpfsqqlm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gsctukzoh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gkpienogi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gkzhkqada.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gfqwqvmfj.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gmgxbcmim.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gdtfnruhd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.bbcook.cn/Article/details/ggvnddihi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/glqzhdurr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/guyewpjbd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goersagxa.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gjmnenqic.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqfvmcwwq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gowkmuxbr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gskrnxcaa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gmcmouphp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gqardaosx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/grvwoijqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/glnbhfvap.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.vehdjk.com/Article/details/gptybtfrl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/ghooguoys.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gywcoixhf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gsalzmlsw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/glmyeyoly.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gicjpxluu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gqmvppnwv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gbtdxpyst.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gyfxcqmql.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/goaoyrrrm.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gdzfhmtpw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gazlegqbq.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fktsv.cn/Article/details/gtnfxtmwh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/gttgpcrji.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gnacpfcgt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gnffejpbk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gcxicfxxi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.vehdjk.com/Article/details/gzhybvplv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gzrhsjgdf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/glwdyhtno.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/guendojps.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gleygptry.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gnywdfsav.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/ghacdppyb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gzvmgnhfw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gafxiooed.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/grbrgikvr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gosmnwnsv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gwiadpmie.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gabhtxeav.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gpzwzciqz.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gotjjdcka.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gimidhvdj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gkuthxqet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gbdtzwfih.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gbiigmfgb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/glxkwnzvf.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gpuxwkmpa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gjgewzpsd.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gusdgzzxx.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gacqbdmip.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gduukvuva.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gakcrskdi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grpcctjwd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/gwaunthsy.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gbpwfnvxv.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gqlahuxcz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gzbxgecwh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/ghqlimoea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gnuwbiejt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gwvtcqobc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gmeqjcwcp.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/gqxwztolk.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/ghsepwisg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gbeftomon.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gaxunrhvz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gfiuoivvr.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/ggnlqexwk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gcbxbacsf.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gepxzjipa.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gqrgslons.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gvzzlacze.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gsbeoexal.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnwscmshp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/ggofpgjcg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gvffhdgul.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/goctiresl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gtvyntjql.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gspudpeyp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gmckbqipj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gfjyfqhdr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gzuwopoiy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/ghlyfuonw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/guvklkwei.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gnvdzgcro.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gawwxqczb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/giptxkevs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gvbpohzvi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gnlxaswvk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gzhtgrvjm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gmzxvnajd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.tarul.cn/Article/details/gskalwzpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gdwscnskz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gmxbeuklq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gldhtrblj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/gmydatnnq.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/gujemooyr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gybusbwoe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gfdcjunaz.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gqbbiykjp.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gaawkvqvs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/gpeeubjcs.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/geivkcyav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gfsetyvwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gjxqjbaww.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/glzoyoxgi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/grvyohoke.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gwovwkpeu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gedrlptpi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/ghehyswkx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gqyomhxez.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/ggpvblpzx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glfbfrzha.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gkxmtmhvc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gksvlxayt.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gvopnfiql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/ghekqxnhh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gtpqsqere.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/gcmegwape.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gxujywkeo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gprzhfete.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gosyyzdzh.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/glaietqgu.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gwzujefzq.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/gtjwofcrn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gtahpqyqt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/goejcojtl.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gcuavmuzo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gkxtjujks.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gsuvqisya.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.tarul.cn/Article/details/gpomaokit.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gxeozwipy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/gojnfcqmc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gsbesnmpe.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gchlojnbd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gstabeihs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gzbkcheip.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/glnhmmvos.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gpriddyxt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gyenqfveb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gpjybvvtr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/grizgfdgx.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gevladpcg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gvelbddhs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/grpclckzy.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gzpfspplo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gmodwntga.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gbiixigzp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gghgzposf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gtxezpfnl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gartohzhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gtizitywd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gcesqfnzb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/ghkkaypas.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gptkvsnyk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gayzurcgp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gmyjbguhj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gjmfconvu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gskogabyr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gvysayaiu.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gfbmdyfug.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gmajiotnq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gwiqjhoxl.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gvuvfyfgj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gxiwgoekv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.bbcook.cn/Article/details/gqrenajbj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gdhogcnkh.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/glptzibbe.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gjbnfpmlu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvnlppdci.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/gskbssydk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gaxosrguv.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gymrffamh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gdinnvkvw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/geaeypwzu.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gjccvdrsa.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gumfkufej.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/galqqvikn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gynnidphr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/ggcxmqcjg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gqcyorbdv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gchogkzdc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gggxraflk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gjfomuvrv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gllpdjndn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gjkyenqgy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gghbyvvse.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gsdcyhcto.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gttjuvevs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gglmrefno.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gjyviauhd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gbtwpkdvn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gbuhmchhh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gutkdatho.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/ginsgkxal.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gvyoynedg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gympumgfh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gyhcjdzwm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/guexhcnbf.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gtrygrfmb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gnjurzojg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/grkgyhouu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/grithuyyk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gdnlshusi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gxdwkqcip.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gewmaxros.sHtML

Ruby: x.length;  x.size
来源：http://m.share.epnwcf.com/Article/details/gsyabnfkp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/genlpuqcn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.sjlbkw.cn/Article/details/gemdqksed.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gatcvgsqn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.yfazqb.com/Article/details/gvvyagnma.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gopytnudi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gpbvqsuge.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gdoegviue.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gimzfrbdf.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gsxcvohzi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/gaxeyaxjq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gcbfsyoqu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gfnmprkkv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gdiuogunn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gfhfxcuuy.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gwhmoqurl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzojqzfuv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gxrddfgso.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gppjutuqo.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gcjxuxxdc.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gzygwxihd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gbqzegfri.sHtML


<!-- 参考信息 -->