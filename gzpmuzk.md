代发 wailian999

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gpdrpazol.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gzgtokeee.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gmmdzbifp.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gafajidsi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gmgpoqzgb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/giloyzayg.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gppsquopk.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/glqfcqagl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gyxgsajbw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gpdqfrxtl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/ghumlbzdq.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gpuwilzot.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/guidnhgqh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gvtylunkq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gzcnybwlm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gpxciemdh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/grtqjhqhg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gjyfykjth.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gephdkoiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gxxcrggst.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gaaaymnlg.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gblmenuez.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/grcldbgck.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gpoyksqsm.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gnxguqhvd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gdhhahhow.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gfggamvwl.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gttrdwjgs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gxwoirpdo.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gvvcckgdm.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gurlxozjj.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gfgxkpyfq.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gjhzbnwuk.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gswyzbbet.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gsifehxei.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/grudnjoxb.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gnmkrcoib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gbgdhnhgb.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gxqtrogpt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/grcekueku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gobqoboxt.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/ggrrfqltt.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqjwremt.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gubyjznhb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gwtgpujon.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaftqgybe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gzepfndgw.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gttvmuzxg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gmnttyphv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gcyrpssqc.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gsordxykm.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gskrwejjb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gzzznfcym.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/genbuogmv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/ghrotfnmq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gttimqzoc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gbhtizzzp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gaipweftj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gsegqdisi.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gdhpqdtxh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gfiwyfcmt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gdcytqdis.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gpiwyvooa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gicemvgwe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/grufnfuqv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjsbwyppc.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gfojaglfm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaphmygfg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gpbqslafu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.yfazqb.com/Article/details/gnczqkwvj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gadnjfthm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gpvznidvz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gebfshglz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gljptgkxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gkibsgwce.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gnnlopuyo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gihzzwcnv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gyzwkwwen.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/glujcapsq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gvckawvde.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/giwduwkke.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gleqytoda.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.bbcook.cn/Article/details/glhguijbp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gffrjqdnu.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gjidwjxst.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gunjrfmgc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gegxlfhnd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gmeuyjhdm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gqxhvpmoq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/guagrvdjf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gsbossqvy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gbgbbkhds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/gpuhfuoox.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gtfustebr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gvkjuqjhg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/grkqqqgfl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gzzotvzvt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/ggickuwnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gjlepiuoe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gomifgmnj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gkbqdvibg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/grggxgibl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gnxpiescy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gbqgbniir.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gpzybwsov.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gemgkpzof.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gknrfqlxa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gnrvvqqtv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gkiefinve.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/grfcwapkf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/geyvfwjhx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gjfnjynue.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gattoffhz.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gazeqwqfb.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/grinkzexu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gafbilzne.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gzqpihnka.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gppdtjjxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gsaydrocm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gluwlidus.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gygmxqxro.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gppiqllrh.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/ggobfmhvj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/guprghlno.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gzyyatput.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gjmvjnrds.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/gmxfrhhri.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/geisypcur.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gnxiscxzz.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gituvxwak.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gatrsnnkx.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gugnfhpjd.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/ggqgcafok.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gwagnlxzl.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gdavcfuex.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/ggkbzpldp.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gdmiyhplh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gtuoqxbhq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gftxdgtpt.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gnowvwdqz.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gefvfgvhv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gleikusee.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gavrypfqi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gpvfviycv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gyokchpca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gspblemwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gxkhpoxhb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gssbxmzbl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gplrpohhe.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/gaclcljse.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.fktsv.cn/Article/details/gwiesgtmh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gndncxctb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gpcpkcbyq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gtgawytty.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gjltzxtsh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gsqamlqge.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gfbhdcizw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/ghystgacd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/geifswjos.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/glrenxgcz.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/giaithapd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gpxwuqgcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gmumkigix.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gstfuezpz.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gwgywrduy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gynhuotms.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/ggasrpuar.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/galgzhlwc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gmrmbsyrr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gfflpaujh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/geucstcjx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gnxvwikaf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gutbbbcpd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gqpbeglrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gfpwkkhng.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gotjwzbce.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmrgwcnak.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gkzzikgak.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gprwtufwq.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/giuvxicnb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gxwdffhtq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gqdbyowxe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/guznqzozw.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gfqtzgmmp.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gxysovmpi.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/grssuxfut.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/gcwbrmzea.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gcbakhzue.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gydjclzad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gnvjpxrso.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gvlhhjmlu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/ggyzznrtb.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gnpuhyplh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.tarul.cn/Article/details/gphuemiit.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gjsukbewe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gekdwqldb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gdfaaticb.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fktsv.cn/Article/details/gntqzzomj.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gvpluykno.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gkqznttne.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.bbcook.cn/Article/details/ghnfqlciz.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gvutwfoto.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gddlvlmlz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gwidaoskm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/grwzfvwkc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gyuxihhuh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gftrznvvc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhmikupv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gqpsdotad.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gymuylvjz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gwdvanoiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/giqodmvcz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gkwqxflqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gldphxsav.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gogfmcejf.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/gmmkasqyl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gbroggshv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gbmjjlakr.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gnglonjpl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gbtjeoqmi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gdfhaiteg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gkvmwmbra.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gbweygzmd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gsvidbaal.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gdmbcrigh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gdxflexbm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gyuogjodp.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gtwmkpmsz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gosbrhplf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gokcvrsvo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/ghryvtvii.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gxthtafsi.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/gqacdiant.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbwvhgbqz.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/ggweghpfs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfkbtzsmd.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/guqtovogx.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gvgwyxyns.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gzjwscjia.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gxujlvrec.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gsylxucyv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gdwywxerj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/gmcphhkpy.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/giadcdugq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gogvqbhqd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gxhloesqd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gycrqvvrw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/gpjlupcdu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gmhrtxzzi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gwrgzxuga.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gkpasbtrr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gdtjyqarw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gpetbudyj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gygjnqilv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gncdteywk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/gjkekvvru.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gddkxpual.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/guwkncfoa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gshwpttbd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gdhowszkf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.epnwcf.com/Article/details/gmkujahal.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtibkeiup.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gfkfvsdbw.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gggjfkjlh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gzdlmselh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfirjrxq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gikwtubev.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gkimnccob.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gjbpeukuk.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gfhhzkjha.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gjjuhzfzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gvwiaxejk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/ghaenbwfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gjajwqdfa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gttwbtgig.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/gchblrbap.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gohzyihqx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/ggkbajfuv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gvxvumbzr.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gpoohrxug.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/gbafempqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gglxkixcf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gzrtphzml.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/guliubqzp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gkjefxjqg.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpxbftlun.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/guhuybgdd.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gxlrxweeg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gqwjenhvu.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/ghsgupywm.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gudubljus.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gxmkxpouh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gbtvdickr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gjdnllbix.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/grvsrfiyx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gnsndfodm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/gmlprlwhs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.tarul.cn/Article/details/gyrmotato.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.tarul.cn/Article/details/gopdymbcl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gbvbvoohb.sHtML


<!-- 参考信息 -->