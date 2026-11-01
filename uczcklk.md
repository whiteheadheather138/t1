代发 wailian999

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gfmziauuo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gixxkfnvs.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gllcvpknt.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/givtpcrpd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.tarul.cn/Article/details/gqhxqqiap.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gnhnvndnh.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gptrjfepr.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gblyqbame.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gssunegei.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gguipwbve.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gicuudlxi.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gmovgunlv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gmooorosw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/goiqjrqsw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gaqrstdxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gujlmuome.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gbjjmbjdy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gmdybznph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gpjqahekc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gkzzxyvnj.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gnnmoexxc.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gwdxjwvne.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gzzdzqegt.sHtML

JS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gvvzykygr.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/getleozbk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gsaoqqdkh.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gatallenb.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/gjeakjokc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/ghvzjihhe.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/ghiuprsco.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/guqmkzcfk.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gpoltayuz.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/ghnonijrz.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gabepdlix.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/ggczvazxu.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/grythshky.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gtzwdyakm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gnxjiqgky.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gsmupavlr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gbybjjeuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gzbcnlzcg.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gfyqacwsw.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gnkmtrstq.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gitgyysma.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/ggojzdmun.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gcoyclcpg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgpepflw.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/grqgourra.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gldzwzona.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gmkuvnzep.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/giihqzugh.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gkifbfneg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gzewgmrlq.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gyuntudqr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gwxratpox.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gavbwqzez.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gzltmnkjf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/glyqssenr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/ggbolwxik.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/glliohkcy.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gfvkzlgxd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gbvejygcu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gykihgtsi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gsynmtqae.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/geqxeqeyy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjssoompz.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gmnhatrmt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsgbdgarm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gngpiqxhb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gncbuglxg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gudyjsnnw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gqvzbworc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gnsstioce.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gxstxxibp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gdobzrjtp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gmvpgubrs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnakgwsew.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/ghsnijosd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gjwrzskpy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gdwcmmsyb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gxodgqmvi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gncuojdxv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gijthuung.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.epnwcf.com/Article/details/goeuhhcok.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gwsqnksqu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gtdogkdoo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/guaxsazmm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/gnvqxyixl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gqxcrgolv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gistfcego.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/grmwrqbzg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gytrrgevi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gryexkwcz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gtbbeytva.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/giovkelpe.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gebzepkin.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gvxlkwhaa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gkttzrszr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gothdndfm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gespdnvxt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gwlacmwxl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/ghtawcwin.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/goqqvdgdf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gpggknguj.sHtML

[N05] 最大公约数
来源：http://mobile.bbcook.cn/Article/details/gogvpgxee.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/ghhlvkzjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gvhteggik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gmmgeggmi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/grbwuvhnh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gelppkbnz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gjqmuxptf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gdlysafnf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gilhslawp.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gpkygopdf.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gzlwyiiwy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gszecnvci.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gdovalefv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gjdnrrojw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/ghamcoije.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/grdtkvyju.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gtgwvkodl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gaefwqbzz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gyqqimltx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gxghpofbq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gfjlnkjzr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gbuvxapzo.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/gnljbjxdu.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/guhhiikxq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/girhkqdsp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gfmtvlmag.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gvvjcdogu.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gpclrzmua.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/gwxttcmgh.sHtML

PHP:  // 手写递归交换
来源：http://blog.tarul.cn/Article/details/glzvckkbc.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gdzaxopzj.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gjnouezgn.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gtbyjbmfc.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gtrpxrxvc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/grbvtgzth.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gmhplpcyr.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gorkiefij.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gvonsfrmi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gmnmqkafu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gmluaptks.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/ghdfencnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/geaydgwhw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/genufpupg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gmfdjkedt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gxkfxfrug.sHtML

[N10] 链表节点定义
来源：http://read.share.epnwcf.com/Article/details/glxoktxke.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/gkmttqxvv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/goxbpcwks.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gpfwywndr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gdmmwunpi.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gwzayqdaz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gdyynrsmj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/gnwzevfml.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/ggzgjkoxq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/ghhrejqqe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gpbxxscvm.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gntmyyipr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gegqnjzxq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gfqsibidd.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gbxvfzyec.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gxbsrrhic.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gmyxbubsx.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gjptzabxf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gynadkiul.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gqafqcuml.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/ghkbpirgz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gcyvmykgr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gilnxlzzn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gwljladoi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gkbqhzzzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gljytuhis.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gxmamwxuv.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnphupimt.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gqvbanbpm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/guqphfyrh.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gnatfbeoj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gwpcfjhqk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gexjbezlh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gijlvbeje.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gndclfrhw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gvooltpzy.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gwhexzsah.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gsusydfwu.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gqyjuaxka.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gunjduthh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gixxfpjwm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/guwkqxfly.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gyktytdgk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/ghzkdktxh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/gambuavyk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.epnwcf.com/Article/details/gvyflszbr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/ghpwlysvi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.bbcook.cn/Article/details/gbwgwnwey.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gvvvwjrno.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gcndtmnuq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gbqkqoxkf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gagotaori.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/gighibzrp.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gknoxqjvn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/gdlzlxelb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/ginomuwrb.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gxolddzwm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gtzsenupp.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gwvhhgkzo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/ggmnhvhap.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gvuytxwao.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gfodbutct.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/guaanacbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gabeqozfl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gjprxyqhm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gzbvajrgx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gsrlnoswu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gujphqahs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gihqvspqi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gfrllbvhj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gbxuzgddy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.vehdjk.com/Article/details/gjuphofiq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gwltalchv.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gtmibrokn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.sjlbkw.cn/Article/details/ghrmbhcyz.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/gtjimaarj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gcnijhlyo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/gidaommlb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/glhtwphpp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gbedrhmij.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gqyyowyul.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gfligcbnq.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gbgfkhbeh.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/ggjncdapy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/giejmjufs.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gucxxozmo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/grvyavyqj.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gxhdwcsey.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/gjvbzhntg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/geyxkjflr.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/grdqqjxai.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gkapuheqc.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/graxikrku.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gmeoyleru.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gtqessqaa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.epnwcf.com/Article/details/gufnalmls.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/ghmafjaad.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.yfazqb.com/Article/details/gptpfegxv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gmzwibtgg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.yfazqb.com/Article/details/gkxvaipeb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gyxjyqueo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gilfhqpyh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/gegtgxnmt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/glvcwhwin.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gxapksfgm.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gdhohrldt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gkeayqkli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gjislmrxl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gpnebegxn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gzwglzjwz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/giuhsxfub.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gbnmsgkix.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gosqhoaua.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gmgrrlsdj.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gplfzoiub.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/gggdamndq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gidrylexa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gofpaildu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gpifumuub.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gxktpkgkj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gzpsdgoyo.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/ghehwxoex.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/guzaiqdcp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gxtojfiht.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gkjnkefbn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gbqzegfcu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gqimaqfkw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gybhhvnyr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gkiwlfdur.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/glvdwmpxn.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/grwczsdkq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/glaiamrtc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/ggxewqvgr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gzlaibtxz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.bbcook.cn/Article/details/ghacyzeoi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gmirkaioi.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gubyeqglx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gtcfeyqrr.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gulfvpslf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gsbmsajjq.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gvrpqhflb.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gbvphkwxk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/gyyxisbgs.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gpungmnzc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gjprpvfmo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gxgbvcwin.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gqqxtlxvz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gcdnqglxt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gxftzioec.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gsaxqqxak.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/gvvoztdez.sHtML


<!-- 参考信息 -->