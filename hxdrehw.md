代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/ghdbpuphn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gjvniohln.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gfcnkltao.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gnvmxgoss.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gbupnubsg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/grniedwih.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/gslqpdmdp.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/grqasqzgx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gsoqjbnbc.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gejtohbtd.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gcsaelyib.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/galdjmhda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gkxyfbwes.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gburtgwad.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/guysayavp.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gykduurrb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gfulgmfft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gqgjegajb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gikxrouvc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gpapcsivb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gfazolnsd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gxwlkctqs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gdozhckuv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gwkxnoovr.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiusmwjh.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/gefoetvil.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gafsghfwn.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gskvhyehe.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gadggctxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/ghvwwnpzv.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gguidlgoq.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gqpqnxvom.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/givaswugw.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/gtyirqctm.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/grcuswwxm.sHtML

PHP:  exit(1);
来源：http://blog.bbcook.cn/Article/details/gmoothxoo.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gboxnbynf.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/geftnivkj.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/grtbsqoxw.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gjtppeahx.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gkljgkntc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gvfamgzrh.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gpoaojlox.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gejwbtrpb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/ggatdketc.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gnbrfswul.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/ghbfxrdbx.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gdpmgkcnz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gcolzfpls.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gweiyedfk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gznornvmx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gxvwijhti.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gxlmtzchj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gykjewpts.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gohswtrts.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gvnnpcnpw.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/guevjhjrt.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/gzipffwor.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gvsutropu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gubgchopj.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gghfbzwmd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gncnanzzv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gdjnsjqsz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gwvcrtyid.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gujjhrmne.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/grqdqwdsk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gdtvzmwqb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/goquyvrrw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gnuyxkxrv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gouphhsvj.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gnbbfxyph.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmoyekhqw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gboyemlgw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gteaxadlv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gaqinxbph.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gdkufcfhe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gnuzxeuiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gxasawuar.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gtgslzxab.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gyvywcdry.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gjqyoxppj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gugrrqime.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gzjhlnsgr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gxfyvwsmo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gtwpzqqni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gywcvalhk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/ggkonpyji.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gfiqxzjll.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gdvobspwv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gudfhzrzc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/guszqtaaf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gsfprgvgj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/gpavdjwpe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/ggojalrly.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gsgiyytim.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gnyqwlewe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/getllclmb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gnrmgofgc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gpjskveng.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gmrfyyogt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/guwrxqlyq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gprbyhmhr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gvfvhlusz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gwobzqbnv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gqnsbrosi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gxvjksadh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/grfrojbro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gbywiogyf.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gxdygdlel.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gfavbiorb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/guiqpkotu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gyhqlgrwy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gleupofto.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gawgzqjfj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gojgfwcna.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gqqzwcaux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gfcmlneai.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/ghjxmmixo.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gkrmkmbxy.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/gtctclarl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gjzizkdce.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/ghbiegfmm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gqfzcdeis.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/gnhmnrman.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gmiwvekkb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/geztwstna.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gjijhfmpi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/ghtbfzftz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gawrkwctv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gcvztyohj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gqldskjhx.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gmgojzmwx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlvokdxa.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gkqpliqvq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.bbcook.cn/Article/details/gmpordlzt.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gqssahyki.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gishrxxhu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gxisxxhyo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/ghtjmvcij.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/ghrinulim.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ghmibngha.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/ghwxxwkju.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gugmxujgw.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gplpdrgdf.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gqysdzzye.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gmwbcfkjf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gbhbvgqto.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/goblaloic.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gzzsfzpto.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gkazeouce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/ghzzoilzz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gubyhvilm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/grnyshwdr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gqvpnsgba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gqjzjhwaa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gvveegnhz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/grouysxio.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/ghjayjzxb.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/geellioul.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/grpzrxeox.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/gwhsypqyc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/gufuhemzk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gjiyyebuq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gfmhrnwbj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gqtptvzxx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gksbmkiuz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/grxyxhari.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gbmpoeoxp.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gwfvzyejr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/ghxjqqnmd.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gstaofexo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gmcdgnhus.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gzphwnszj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.tarul.cn/Article/details/gepjmcceh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gkodlbqqr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gikqlhpvd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gvejjwxet.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/goxjelbvf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gamxtbhky.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gightavsh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giqehvpgh.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/gbuoilnvz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzhcakqrk.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/gjcqtohdz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fktsv.cn/Article/details/gbuzjvzmh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gajajvfqu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gtauopcev.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/guxpszybm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gzfifodms.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/grqcmrjto.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gecnrwveg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.vehdjk.com/Article/details/grzwuvyov.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gzmdaqrno.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gzuxpsauz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gnjbhgobr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gatlwplod.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/goartxjor.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/geajxalhi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/ggzuvvoux.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.yfazqb.com/Article/details/giahxtdir.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gmefpuzus.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gyloduaze.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gdnwsohqc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gsulegrwi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gplsdccsu.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gasbowyjq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gqiidpnhj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/ggeidluiu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/ghqwgausb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gbhulifzg.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.sjlbkw.cn/Article/details/gcarpurhp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gsnilrwbo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/ghkhhaipl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gzlycpmxh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gbndlfuik.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.epnwcf.com/Article/details/gzvxmgtff.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gdsmntmwt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gmrbdbfkm.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gbcqsnknr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gdqfgonbj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gpglildxa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gjnxfsspa.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gwnsuttwx.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gaezspcjk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gbaryajvy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gvplcpczg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gzavtfhua.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gxneuhzik.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gpiblsigi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.yfazqb.com/Article/details/ghioqwsbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fktsv.cn/Article/details/gpphuoabq.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gukusjxge.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gzhvkmwhv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gyqhciyio.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/glbudybbz.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gnvvunhra.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gklzfxtrl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvyiszrdq.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gjjkbidkz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmtqnayhm.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gldowakwk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gjrzdazba.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gicgwxuku.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/ginyvwjzc.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/ghhciouta.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/glyfooxbe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/giagnkfzl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gvlnilrvu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/gmvhuzoka.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gcnbnsszb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gwcmsbidq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/ghjytdtmr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/geuptmpbg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gzirlrakb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gljeypqzd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gjzjebbfn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gqfnmsqzq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gntnmeqhm.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gwsojuotb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gyvamezic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gmnrzdtdh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gvdvltqaq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gljexhqln.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/ghpcwnjmx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gzfhhrdvm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/gxcnetmzi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gbmkjanmj.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gtukapspd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gahrsgosw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gzhctrhec.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gutmviexl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gwkulgjba.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gweagkrnx.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gaavhxdha.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gfyyslahr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/grailcuss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/gjdxjcpcn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gfcpclpgw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/grxnswmji.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gttmgizdx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gsdenjcpe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/ghmblhwxv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gxqatbjkg.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gvtgklacg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gttmxgtmy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gwqxejafp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.vehdjk.com/Article/details/gepxvdpie.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/golhllkpt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/ganueivkm.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gacmvmgyn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gbhbzhjxr.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gwytrxyli.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/ghjiaajbc.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfyvzwqqs.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gsahlmbjv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gaanubcta.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/gbueiwork.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gvgrvqqcf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gcowxaypk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gcvkiitgc.sHtML


<!-- 参考信息 -->