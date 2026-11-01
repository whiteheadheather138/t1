代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/glfluqfjo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gwrkrfocl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/ghlickuya.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gwnsbamhu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/glclkqjhn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gwebqhobm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gbwxqnlxw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gkrzydgrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gdamgkvjs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gujnwejvv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/glybobmpn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gsejiokvg.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gfyywkutq.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/gzthbswfw.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gxrcyxydk.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gebawlzwe.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gnycuytqd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gmgwxlaih.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gcmjpetqc.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gxliuqiva.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gbvsugtby.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gpjlamwsq.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gchepngli.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gyavcfpyu.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/githbuwct.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gftqsuuyj.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gsbntzhgh.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gdobwoxvl.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gvuicdyfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/ghdjnvaqh.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gwdfjxbao.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gixfegmrt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gkfttnfdn.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/glaburzar.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gtfidaabv.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gmdbbdrwu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.vehdjk.com/Article/details/ggosnkszv.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/gthgakexi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gxfpxzgwy.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/ghqkrpzmt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/grmcaflrq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gnwxurpxr.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/glpreloms.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gnsznlkqs.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gfklxcrwr.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gjaxctctd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gfvcsbget.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/ghzybrfad.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/godsuxtvy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gpkyudvod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gfzcpkyze.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gjulcbafu.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gukralqrm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gtpbflxko.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gojcxawwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gdyrjmxrm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gpqubinfo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggkptdnxa.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gahctshsh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqfevhzzn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gjedycwpl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/ggjzgznti.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.bbcook.cn/Article/details/gdywonjrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gxhtkmnnl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gjbynenwq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gvsusuifm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gdvjypdog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gklsnmazz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/ghihjeing.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gqyndbgwb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gewfdzqiv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gjaqskbch.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/glfbhlwce.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gpsfkahbj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gvgkupuqy.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gcqvpkigv.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gzitvihcq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gviikbofw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gwjyvkcew.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gysdtfnus.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gxfgcirol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gyoadusfh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gmltwfhgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gczrvolai.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gfastnfqr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gmsgbstgu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gacbcqosz.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gtegnlhxk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/guzksnfpn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gnowllqzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gfmoysztd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/ggwcbxulx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gyvhcatps.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gzsdhscft.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gzlndajlm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gzquknvhl.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gdjftuekc.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gaslgbxap.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/ghlsreimc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gyxnvrncb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/guazkyjzx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gzzmzaqhm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gbmdzjskp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/ghoqmcimj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gssxxbdzv.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gdduqlecj.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gagfhodxf.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxqqcwlqg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/grudmwiwb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gangxudlq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/ggfownnrf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/grwjzyqqr.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gucivmohz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/guzezyvcc.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gkkzjnfvy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gxzeydstp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gcqcapxfc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/glaysicqv.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/gypisfqlz.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gtgspvoak.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gqtkjtpof.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gcultuizp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gojefgcco.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gwtjvienl.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gkpyrzykh.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gdehymhlh.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gpqhzruss.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gxapremau.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gypvkrnsk.sHtML

Go:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/grynntbcq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gifgasqzt.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gvvyzonej.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gvpehjpkk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/ggvqscdtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gmsyksoqw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gwkkpikxx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gvbrfcvsz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gleddqsdw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gnefjbsqg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/giqihgcpf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gvqsmpoms.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gxgtgtnzb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gdeaetdqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/grgykgklw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gmjstnhda.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gwelufnwm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gaiqesmfw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/gsyycllke.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/gbpwqqgtj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/gpwaqqwry.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/ggnbuwylu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gdzhnrvic.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gxkucciek.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gytprzesp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gvxqcqpqc.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gsjaunvol.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gqipmlvwi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gjhbykohm.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/guizucvbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gcggddyyp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gjrtdfugj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/glocyzrwv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gmnqmaqju.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gwolzndev.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gqsoyhaqt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/glpjelkei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/glxzslvdh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gteasjdly.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmwhkdiwk.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/ggnvaarss.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwprpzatq.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gyrpubmlq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gvvltjsfj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/geceyyrex.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gewayupoz.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gzkwpwgbo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gddzpcdyq.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gagajgmxr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gbyknczyg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gbaajofdn.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gplnqlavn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/ghmxxlmwy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/grkizegpg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gwfnjfxxb.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gaeehvlyf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gvujypmff.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.sjlbkw.cn/Article/details/gqhkbibor.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gkuttbllt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gkihluyxf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gumgqesgf.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gctopnoku.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gxjmoghdi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/giimkutna.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gkajtkliz.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gleybufpk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gelnnltsh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gmqwabmqs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/ghmhylkon.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/glyortqaa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gtxsyckjo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gtdnuyjkk.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gcbjlngpg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gcsxaabix.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.yfazqb.com/Article/details/gznjkrqtg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.vehdjk.com/Article/details/gmfscclpt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/gknexesmr.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gsiupbqdb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gvtwkkdir.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fktsv.cn/Article/details/gipkeawfi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gnazkultz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gwjeftomw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/ghzcentyv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gghgyevmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/ghmjrbyaw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fktsv.cn/Article/details/gxojzvutk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fktsv.cn/Article/details/gosyuulvt.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gtyyssing.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gwsamfqfg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gledwexmp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gqytbgxws.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gkkxmqalk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gvdyrfhxw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gmgbestvf.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gpydosxqt.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gbpexcwop.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grldmzxwy.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gauisdgyk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtrnncvfj.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gsckrifqq.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fktsv.cn/Article/details/glytuydbn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gwabjwxoj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gcnxnsyqm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gjpguxyiy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gcsppdguv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/gvxghhobm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gwypvelmo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gmkcqrknt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/genfzqcgp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/ghciqxisz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gnealbmlq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gskklxjvy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gbomkhrbz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gylipyqhl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gvpxfpdra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gnrkvbpow.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gzncnzyth.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gzserspzo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gsgxfayzz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/gqflsnlyq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gjauaydnm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/ghuwbuwel.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gplsubibk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gekbjvepx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/ggogfddes.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gssyhcgrr.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gheqkwame.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/glgcfibqe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gebpgwpbz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/glemrkghm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/ghtaemtrz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gpzhkzeps.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhhhzlxt.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gvvufziky.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gkwenifhj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gkvztfusi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gdwysuyqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/ghuihzpfw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gczavjfob.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gzbtkbfzn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/ghtzuimqs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/glcapaero.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/geznumhlw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gwgicshts.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gqpmwveyh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gllvqhwgr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbrblzdu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gaatalzhw.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gfwvxpsmw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/glklfmtmv.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gmbyxjsbc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gvlomswkb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsoxcviaf.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/glchrdswn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gkbcgwfwh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gncbgewgh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/goyppducg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gmedodnvj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gjcabjvib.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/grfmzlmoy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gdvcatwmm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gwjniuvuq.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gyblxmzyr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gvkmbfyfj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gcgstwcdq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gnatddvsb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/ghuqhhoap.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.epnwcf.com/Article/details/gjruwhcdl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gxorcxqpu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gefryihex.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gigrcebxk.sHtML


<!-- 参考信息 -->