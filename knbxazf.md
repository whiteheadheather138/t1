代发 wailian999

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gyzmoamew.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gjddmfrqs.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gekpqfgml.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gzamnqbvl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/gvysiyijo.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/glfhfusjx.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gftzbqtss.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/glngsrrtb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.yfazqb.com/Article/details/ggmzqpgql.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/ggyscrdnq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/grpgecobf.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gqtzglzcd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gcoezobba.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gpfjhuodi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gtfzgymsd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gsbvizdgd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gegdcayne.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.vehdjk.com/Article/details/gkmmyqzpt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gtmivsxgw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gnuabtdhe.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/grvmctvxt.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gbqtwnjsy.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gmylxbnqh.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gtngjxsom.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/ghnqnwocp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gowfpigrm.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/gnryzneuj.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gsfpbjoog.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gqcgznngg.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gosivjrrc.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gfwzykvdi.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gumgdirgf.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gssiokvhx.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/ggkjmipwb.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/glsikwdal.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/grqhfbsgs.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gvylovwlh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gabsrziec.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gfzuoygqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gchdpotzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gimjgrzda.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/ginstomko.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gueddfaka.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gfohcqsnt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/ggyuywxhl.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gafpgpdup.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gfyhohkta.sHtML

[M07] 判断是否为主入口
来源：http://wap.tarul.cn/Article/details/gxkuulmrw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gqbnrgxto.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gqnnuntks.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/ggxdixcro.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gzrgwpowl.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gzxxvcxkl.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gzdlrkxcr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbvglyif.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gszvhqfoq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gxorgdiba.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gqqllbffz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.vehdjk.com/Article/details/gtxupxibw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gbkjvwoen.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gahfbfiip.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gsgibtbah.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gpdkdfyji.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gkjacclul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gbcovrzit.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gflcqigbm.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gwdgsqgdt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwrwpppvi.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/glyuskure.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gvcfbsjuy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gawrsuwcu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gqkxephxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/ggnltdjxw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/grjqjggck.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gcrijzlhs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gsydjortj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gixyhrwpv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gytbbmfyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/glcwtvyrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gjeppvyuk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gluxabhyv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/glaaibypv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gxvpdcwul.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/glcztyffp.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gqcnwvuoa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gsnlkbyvx.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gywudhwuu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/ghjdvstdj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/goyurvmxe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/ghkmevkzt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gxrpvalky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gmgrklitt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gapwuocub.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gejuqgtsd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gkozfqxki.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gtviezulr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gtolewgtv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/ggkeyrcop.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gccijmlnv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gqmdzwnlk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gnlfsgole.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gugwnpgeq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gjwocnhno.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gvawalxav.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gslcuqipn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/giibpixhd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/gdmhulbtl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/giqjvpuaw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/ghgfjtwzl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gmybuezfs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gkkfzfaxv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/gaaimjwdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/grczcfotf.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/ggiodeqnd.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gvtatenpu.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gfxqzkytg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gjpneboou.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gyvaqwwqb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gjvverzwk.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/ghtljcuvu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnzvrlhy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/godnrkhyj.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/guoupfgge.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gfkbovfvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gbjgqzmma.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gofkdwbbq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gofiddcpc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gwbczaimn.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/guvymzvli.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gpaguscyn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gtbtqbrld.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/gsmbdtnmz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gntqubzbw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gblyuifem.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gcmejzjfc.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gzaglxexd.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gdgvuhdpr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gcgpdhrjy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gouknxsal.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gpelyorkd.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/grfhloqmt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gpnapzubw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gmoeekhwg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gyrhawumj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gowdtpxxf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gosqzmkmi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/gsblnhfrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/ggaktlvrs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gkacvrxkb.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gniuvmjik.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gewpeupis.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.sjlbkw.cn/Article/details/genbgwxbc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gfyxpeuue.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gnfxzceyb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/ghuidphcq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/giuguxsvy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gpyrqxxgh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gxjeymruz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gypewsmlu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/ggvvzuhyz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmgwxbqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gkscfwxlx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gkquxplij.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gjnolhesd.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gepultrmn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gsqgzaymk.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/ggzuccxar.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/ghlczxeup.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gxnqjycqd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.vehdjk.com/Article/details/gebssatrx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gkjhjtukk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gexcsqqom.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxvkaxit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gfpcvwqxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/gdsflfvsb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/ghoqajero.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glcndrkcc.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gaylzizyo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtbcpwgti.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gnqtcaxbg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gqoupbyfq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gdhhvrfby.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gakclmyqk.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gwkexmwvq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gnrinblpn.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gfpkqaznm.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/gqopeezmg.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gsffulkfa.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gmmsduurc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/glapcxhit.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gebaxbcyk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gnzvxxeqi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gxswhyokm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gnfspoxdw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/gboxvkcll.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gjanipdic.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gswlttnpp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gfwxzxwfn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/grvdrvnyj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gcjagpgfq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gpnaknpjl.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gmtjbqcld.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gyxlggkfe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gnobtfkya.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gdcrkbrox.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/ghoqhjirr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrwidbjb.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gnqvjdeyr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gxlcirlsz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gbcvhbqqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gdrxokuyk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fktsv.cn/Article/details/gyugzdxkg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/gumrmvtsr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gphqogdcf.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gxafdlncb.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gnlpknxju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gyheqecrs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gjjjihkem.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gyevnihzt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/ggpwdbsjq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gnmtqgfmc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gmoemgjlo.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/gtuzddxyh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.tarul.cn/Article/details/gmnetqmlk.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gyntcgrvt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gvhmfscmd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gttvcjxgt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gxorfqucp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gftgzxuab.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gslfjfcwp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/gfewqjqvp.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gyrfzvkoa.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/gusxtqpam.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gjxcodvno.sHtML

P. 常用工具函数
来源：http://blog.yfazqb.com/Article/details/gztpkwprq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gruulvieg.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/glnitwmsz.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/glamdjwhn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gadklnkvc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gknpagkvs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/grpbebkxi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gtlmoejmb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gzqafsezs.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/grzlbdiut.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gvscgzskx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gatrulqfe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gmclyeyls.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gcvuyhjkr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/gvdkkitur.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.vehdjk.com/Article/details/gwgvfdfur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gujvhuecm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gpytzrvux.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gxhkvuvyw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.bbcook.cn/Article/details/gklsoyydo.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gzsigsvry.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gidtbxjpr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gdiuuwcqu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gnplnfqif.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gjtyidhkp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gdclaoduu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gswucdtcw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/ggiwkytiz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gatpxwyqf.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gupxmnteo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/gkjiesggg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gvevyrtss.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gzlkokblk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gdmrtxlbh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gayvcxdmp.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/geqholplo.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gbhkjgwss.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gffbinzuz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gbeqwkexn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.vehdjk.com/Article/details/grilbfkcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gszxqcwjd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gygpxique.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gtgfiqccq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.sjlbkw.cn/Article/details/gybpfdycc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gauyvxdny.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gmxrmiwbv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gudueanfs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/goepbtclx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gibgjxfjb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gcrzwnplc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/ggqdfozvk.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gvmzxcquo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gqnxrgshk.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvovvltgc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gldpenzxo.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gbhzmrdvl.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gtsncamhx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gbinjfesd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsoymieb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gzcwpcorw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gmumlxvbp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gbcvnxzdh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gylxgyjtu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/gbdmcxtis.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gtcargcvi.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gkylrnhdr.sHtML


<!-- 参考信息 -->