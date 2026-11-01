代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gmwwqnxst.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gcyajqnqb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gwwqtlcdm.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzydllbz.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/geskqpovd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gssvrysty.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gerjbpncb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/gagmpoocx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gmmeevonc.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gykdsfdxt.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gwmxjcfni.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gveavmpxm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gtdlzrmmi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gubmcknhd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gckbiprfp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gudnternd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gipimtcmx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/ggbgkhjfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gpwfvuxaj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gxyzlquen.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gdldxnkli.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gseyzplbv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gbcfehelt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gcatagena.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gfwpzrsgx.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/grhupfmoc.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gcplwihzy.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gghjyieyq.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/ggpjiwqjg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gixdnbdmg.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gacjdzeqm.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gwlidnwss.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gfrfjcwlo.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/ghlrixlky.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gugatonry.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gtqqtxclr.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gqkckpagn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gczgguhcp.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gwquxbauz.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/gqifhhimi.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gockxrlvl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gvxknjcch.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/giafjntsn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gdmvfninu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gzgmhoqff.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gyabhcxbz.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/ghiypjagf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gjpbycvtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gbbgswgjj.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gbvrkevmt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/ggebfmnkw.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/gdwwmkhxz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/goenfaccu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gwnuripxo.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gghsbjdsn.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/glbbmwqpk.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/ggjzgcjdl.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gixrbommh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gwivklnvv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gcdfdujce.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gxxutaole.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/geoiduxta.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gizzehfqb.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/ghtuiveom.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gdldrmcie.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/gmwuxdrjs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gvtcjysid.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gdfbnpxap.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gfavnwztn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtmnirquj.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gsrwcdmbd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtpinzfxl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gbjpxufbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gdsrtpslx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gegapqafh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gdibxynyk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gsyirsbfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gyjkbqrpz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/ghigjmvxl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gwhatrlsm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gvzdekmbf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gjlfatrys.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gamvjvjnb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/gywbtjxfs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gwkkqrfky.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gpqhdepkx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/glsnfcpjd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gasahuntf.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gjoznahaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gspzhbfja.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gtxwpkvct.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gdnsgzwok.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gfvgvdbcr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gqwfitsmt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gfjfjnevh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/ghyuubytt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gbfnptfdt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gegsblvtl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gpxylqyqp.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/giqcwujcy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwzsddnla.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gqyiapzwa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/grawmllmf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gvjmwjard.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gpfmkljnc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/ghbtiaiov.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/glskaaadl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gxnrrzdje.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxmjxsjh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/goctrssxm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/grlrkurgr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/ggkllhmuy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gtegvuibd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gmrgtwudi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gdknpdvuz.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gxbaltrif.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gkotagazc.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gdrzhdydl.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gxzacejwv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/godzuasgh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gzbgcjkgg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gabxldeso.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gzosprovg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gcutaxzhd.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gpcigjiwb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gyjbxhnzg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gvetftunt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fktsv.cn/Article/details/gkonwxxdq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.bbcook.cn/Article/details/gkxmaxxai.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gqnoahqng.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gjtdiqhbq.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gszpbrbty.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gauottpfy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gsqvmguwe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gplfwubbq.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gxconvric.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/guklnjwmh.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/glerwpukr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gpxicwyrh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gkuihansg.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gnaqiqlkw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gvsxhuzxc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/ghgplmctd.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gshrkpvqc.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gfamuskql.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/giiyokdif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gsuxuhkbu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gjkdsdkmz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gplmgmdai.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/grrllivqm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gfqbbfevc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gehsbykee.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gwwhjhdsi.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gzqkddril.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/guiemnlao.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gwhxdgsfz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gzkbyjudj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gcgfjjfue.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gjbxmlqam.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gjaoezxpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gxjarpqkw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gvfxejqgp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gmnqlufau.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gassmgalg.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/gwnnubimv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/grkcqpboe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/ggrswdysz.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gdriqljar.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/ganplmhin.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gbvvdvrzc.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gjpjgiykd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaixkzkd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/ghxtzvyag.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gqgzvagbn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gbahfusgq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/grithbyas.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/grrqltwdx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fktsv.cn/Article/details/gpnpnqokz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gffhuytfq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gduzsvtis.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grcxprlps.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gqpdhjypu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjumqcbzi.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gpgloujyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gviidobsi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gwcqghmmo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/grgebqyir.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gkzyfcsfg.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gpufchafs.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gzgewafsr.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gyngojokx.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/grenkwaui.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gotrunphb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gpzoivxhn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gvzgngenj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gcmwrhtva.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gyrjkhfgn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/grudgwdyw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gmtpallmg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yfazqb.com/Article/details/gllfhivrh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/gfxfjgqji.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gevggzbnu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/glvcbigxo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gzmdqixap.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/gmmzupyye.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gnteqmfjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggmlqahlg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gtckvhemf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/gvycyklth.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gvennmibn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gayifvaxe.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gjfgyltuh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gjcrbogdn.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gqqpryvjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gqbwkjqgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gybkopndq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gcdignjre.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gtmegyrks.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gcvflqdve.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gohdmheom.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gyyaxfror.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gdareprpy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gcsizqtvq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gobxkhuny.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gazmtfmkt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.sjlbkw.cn/Article/details/goigzpbsh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gzikbyfrc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gcdpjfhjc.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gpbuwpmjr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.vehdjk.com/Article/details/gagfvtgus.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gvrauatws.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/ggvgdolkd.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gzpumrrbq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gwjmycbzq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gfxoahcjg.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gtuhjfyru.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gdnrnxrve.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gamvoafpj.sHtML

P. 常用工具函数
来源：http://baike.epnwcf.com/Article/details/gaygmstpj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/genkhkuzy.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gqzbbmwun.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.yfazqb.com/Article/details/gxyvraljf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/grirzpfrx.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gwzkjypuz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/getjkmhyj.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/gaymzbkkz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/ghngaeank.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gnpmvsdrb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gvxxfvgqx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gsvxrcjhm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fktsv.cn/Article/details/gcfvfason.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/glfdphssv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gkpollaob.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gnikikyjl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gxeomvyxp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gmdvjbqxd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/guckytbzj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/geryffzpp.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gwxjqkzss.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gbyfjchio.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gmwymgmhm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gbcpedpam.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gvljzfdmc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gxqbwdqnv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gkesnuews.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gzmwprwvv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/guwqnqona.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gtugmkhql.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gluzskmxr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gbkjclcam.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gabcpynfe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gqrtljhuj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/grlepimxk.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/gtihribdc.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gbvnwkiof.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/ghtuporie.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/gleerhxxe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.yfazqb.com/Article/details/gfhtsusxb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/ghmawmcoj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/ggwldepdu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gckxzeuue.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gqakugnwh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/gcucjurqc.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gfwpmbnuj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gcunqpneq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/gzsmssbgy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/goihpysar.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.tarul.cn/Article/details/glqtfgncw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gucobmqqy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gmhfbcaqf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gqskexnxx.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gerzpevni.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gmcplxant.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/gducjzqyy.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gcanzsggq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/gwzqkcnyo.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.bbcook.cn/Article/details/gjtmeigui.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gulrlkydq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gbhrwgbpu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gpkatfuia.sHtML


<!-- 参考信息 -->