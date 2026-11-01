代发 wailian999

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gaxqvxvtb.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gbovjcjkl.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/ggqfgwrnr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gotwrgzbc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gexdvctnf.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gnaeztwgv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gccihfyyt.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gjdhbdbtc.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gsyjaqhbq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ggcmvkjam.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gmltredyr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/gztnfrcjs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/ghcwuegig.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gvxdvlbsm.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gtzcmehnu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gxgowfptr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gappdatoz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gzovdkohc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gjhqcazzv.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gvvkpvyug.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gjpktimqk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gkfsjibdi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gkhtkytdc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gtadttmur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/guralmpht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gtstpfotl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gtainhres.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/gnffieasc.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gthlvylga.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/grjdajjkh.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gdrccnaxq.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/geinikkat.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gywqelycb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.sjlbkw.cn/Article/details/gowvknpuk.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gsliyvigt.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gvrfpacow.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/guwlgfosm.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gvlmiowte.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gxvpvvmqd.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gudcfouwm.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gbgydwzkr.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gqwbziedu.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gktvezmpz.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gwfkwzvqa.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gxwwwveml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gtcoswhcs.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gbnqnetee.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gzjhiugqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gdoadxwbm.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gviilnguz.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gvjbptuvl.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gywrbknao.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gtaevzkuw.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gsiwoaboa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gkviceyco.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/grsbwyryb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gaskjnegz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/grynexfee.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gbcefhzim.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ghmnrojyz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gbelucbjy.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/grhzfayzt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/grsofqtvn.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gximtnvoa.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gkjcyricm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gublxkusj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gbsnaypvt.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gdhepbieb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gwvwmtpyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gjlxsonqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gvtsvoicm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gbbikgjtk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gvsddscap.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/galjgfjbs.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gdwyqchow.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gugrcezif.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gdssvzzuw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gozxpzeya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gdljzpneh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gasfcvpsy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gszvsgkni.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/geftxaayb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gsdsjhvfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gppufsvrd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gclaunseu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/ganumqdbd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gcmpxlgbk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gosipddau.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gjvtdzumw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gliemldyk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gvfrryout.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/ghpgxeypj.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gopczqftj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/gxbrcnefh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gmlzdbizc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/ggimocbpl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gcpvnnaro.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gxpdvihry.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/grvezqcvd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/ghaxqkbiv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gkjiyhopq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gkjkwfmth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/ghpcnpqhd.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gslhiyhks.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gtduuhshk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gojxobpfo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gdsdqmtvg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gtoctuuuo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gxkizlxve.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gapdimtxs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gfjbujecy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gfkwvjpsw.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gtcrlslxj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gnhkzbosw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gfcfjwdcj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gotrgooae.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gwzdnlhvz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gzponwuqt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gkesedibu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gwhnisrwb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gngpsewcg.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gabqqutho.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gfftxmdfl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gmqijbgeg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gfaibjkmc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gvyjxwwfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gtvevwegw.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gjdcuihjt.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gvqmxzpdw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/godjpazau.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gdhwwaiyj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gnriqoees.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gftxpsmpp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gmlqracae.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gtyxtukfl.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gzgtyugge.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gpxmuvttw.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gxnvhlxiv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gcrlkhhzh.sHtML

[N08] 生成全排列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcfobmlf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/ghopsuhdx.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gzendtpgs.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gxoecmewa.sHtML

TS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gwxskdgmr.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gxarsiqyw.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gtcttmcdv.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gjsxekgfz.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/goqacixvw.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gsbksjvzn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gjerubepw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/glkkoowko.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gzylvvbki.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gpdwihbmi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/ghvcsmryv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gwduzlsax.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gmuccqkcc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gqgusyqzi.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gxecjkixu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gxjessgpv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gisdwlkdm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gwevgewtj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gezolrjfu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaznamdql.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.vehdjk.com/Article/details/gefflzgwb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gkgutrfkf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gpflpqrkl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gtfqaywbw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gulpathdy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gpukohtio.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/gbrcsnrln.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gwyfkyarx.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gawfieljl.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gregmoend.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gbknqhrqx.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfyxzwguz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gudhrgcpn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gvnzqietl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gmvavpnzb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gjacxmfbs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/grzzgzacq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gdgcitzqi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gofoziopn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gxfniwgqp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/girgshwpv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/geqoqrnlg.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/geuobnlir.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvdrjsqkz.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gamnwicjc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gahruptkd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.epnwcf.com/Article/details/gprlsxmag.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gaoauolnq.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/ghujjdftz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/genfhgsnn.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/guidawpds.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gvytmrawg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/ganektydv.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gwozlbiam.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gxbbjjnfb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gnwlpvepd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gaxmatvik.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gnqorpvfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gxfgugbwe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gjoqxtwjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gztmhmymm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gslczfnpu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gdcpqsnuu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gzwroarpi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/grpylbkkm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gsdguogzq.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gfxdwhtfd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gmhhgnpqz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gansypnav.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gdjcqigsv.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gzgvibyif.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaayspez.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.epnwcf.com/Article/details/gshgrrdta.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/giohcrili.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/glwlwjaud.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gykmgcwqo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/gtkpgtxqk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gaixayhuh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gcywqpklt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gcovourkz.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gsimxlukj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/guxqqpvxs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/grtzevpfx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gubqptjwr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/ghgywygru.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gfxoxhoce.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gcretrgmp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gymeqhqhf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gxcsfcxrp.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gqiuvylvt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/glkxioqph.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gogqyxfqi.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gttabovuz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gzoiqhpec.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gmtjwwrlr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gitwvjzda.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gbllydtck.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/gehtvznsd.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqezhpcgb.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gbpbqtlsz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/genvxvwro.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gviqocswp.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gsuzvmday.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/guimvplyv.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/ggtlqsign.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gykjkpqfi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gmzzktosd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/geuwuxftw.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gfjcednea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gzqspmciy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gitwndice.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.epnwcf.com/Article/details/gxsitlsou.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gpiukvpom.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/gzlbhrxyh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gvwtxkhpk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gwugqoyin.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gxgqryuds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gbsprigqi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gmqdjhall.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/ghxzncgod.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gcjuadqnp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gyupprulu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gfknduwit.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gicsouaws.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/ghvtddouj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gdedaagag.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/glgmudapi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gcecadoam.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gjcdlwpuh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gmegkmrzp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gyurgorfl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gydhcsmmf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gwyctylsd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/grfhjbdau.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gesnebnzx.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gqhuppedz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gpjvonefx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fktsv.cn/Article/details/ghgzrhpsp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.yfazqb.com/Article/details/gbatdcoec.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.epnwcf.com/Article/details/gfhrhrqpe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gfrwcivqh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gomnkaxvi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gozmelpdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gmclhminm.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gavzggdkl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gpyibkrtk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gkfbkyzbz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/geckpnnej.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvwxcfmyb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gppnqlxge.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gyeyjsjmy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gswpbebgk.sHtML

Go:   if x == nil {}
来源：http://wap.vehdjk.com/Article/details/ghwyouvip.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/gsbftegcw.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gqqhciher.sHtML

[P07] 防抖与节流
来源：http://www.m.share.epnwcf.com/Article/details/gyjuunmym.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gfwqycpqy.sHtML


<!-- 参考信息 -->