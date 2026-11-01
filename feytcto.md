代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gbxjmvdps.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gbbsquhwc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gjkbkscxk.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gfhzvvwju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/ghwxsfebe.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/grjctdoxd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqxudtgc.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gialkllcv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gyesspmkm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gupqqrvsu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqynaccjc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/ghzwwffzq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/guniwwsbn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/gqomhhapy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gwkgkmuyi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gdrqkjzoc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/gurzrazpz.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/gxreiokbl.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/grmvilhqs.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gutyreuzn.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/greqofivx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gkkqdtgnx.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/grdmlphhy.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gyttietqq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/gceocpdxa.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gmsnxzhnv.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gazyxogho.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gloojufnb.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gzjamqhex.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gmfrbdgmi.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/grjxpoyhw.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gvygtpcni.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gqtqzpdke.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gtqicgwya.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/giflvgkik.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/glmnvnfit.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gknchndpv.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gepzgjxmj.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/glapyqohk.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/gkcdshwby.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/ghmqugzso.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/ghdzfjhuj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gtdsspeqg.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gzgdzxvpn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gnjdunron.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gregsxfry.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gwaiywilm.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gqrsszzap.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gxrgxrzhp.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gbpjpotgi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/ggwmfkmxh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gqvkaedst.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gqxxuumrd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gqsktwddw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/guuvdiiov.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gmsydhfwe.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gfcunezpr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/gzhbbzzsm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/gygizabpf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/gkhebnmxy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gjcvlkart.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnlefjymf.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gvceacygz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gidjpgrtn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/giafdhbrl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gfpntoqdr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gzrixsnjv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gsoakgpel.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/ghvyuunyr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gfysmcisi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gnqjozupt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gvvwvqpbf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ghctbwary.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfpioxxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gklnjcggd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gjsatdpqb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gvrzrccab.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/guwpdjdqw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/glwdpfgbs.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gclymurqa.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/grbwcgtzu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/goroilskb.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gifzuulbi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/grwdoqbwh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gxcaxwedu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/geatbjepf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gswjgfgnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gstzthqdz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gbozflwvw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gduurtctg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gppydtgld.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gyjwzkzgj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/glsidoaob.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gflnbdyyx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gqfimnjlh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gocnqszdx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/gcjilbnpm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/gjexsdmxs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gcwowmsfj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gmjmtrask.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gjckyyfyu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gqqmiminu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gjcxexdny.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gtwajjmrx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gvyjdczuf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gccolgkpu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gyckpmmqm.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/glrttxojz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gskxnqitk.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvcjclbqa.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gtixdxvqd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/ghcmtnpyh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gyiklfpkd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gyjsdoywf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gejtzdvws.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/ghkgjlptm.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gintkhycl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gmfffvheo.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/ghdldugoe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gxvxbnhys.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gzizcdbmz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gwkubqzxx.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gfwpiidqh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gkhovlnnz.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/guwxstwyj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gonritznt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gjwwokjrm.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gcuaqvqkk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/guysxupkc.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/gglgwcqtg.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/glgvoxpuj.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gcubdkdbj.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gclrvewwh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gyszwukop.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gtulcwwna.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gxxzhzetz.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gbkraqdfs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gpsjthrzm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/godmolnoo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gjxrfdxkw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gcqgsvqzl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gfzzvcaty.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gnhulnvtc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gopvlsbav.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gpcxgajlf.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/glparmbpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/geukajjqp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/ghwbbjinp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gzzrxcqmk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gctvecrga.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gqzszmwwv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gavxefjes.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gknxvgwje.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gpwqljlft.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gkrjbcift.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/ggamlxubn.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/goffbkabm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gexinfqyt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gjdtxtwrm.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gdsawdgvp.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/geuncukhi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.bbcook.cn/Article/details/glaohvzpz.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gqfucdirg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gbhsyrcoj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gvpomjaia.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gzlpricez.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gxkbxhrag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gjklpzukj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gdbnsdxfj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/grlzzptei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gfyqecuem.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/getqnoipv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gitlvvvfn.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/guxryqsou.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqfcxmhhu.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gjyoscica.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/geszfrmop.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gfnvhagcw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gwablriiu.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/ghducqbeu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhihplol.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gmlzvudkg.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gjqyznwvi.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/gnmnclfro.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gxvvcmkpn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.yfazqb.com/Article/details/gnymeegfu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.bbcook.cn/Article/details/giwoaexyl.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gtqddgjnh.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gtopzfyux.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gbgiitspi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gmnkjodzc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gbbflgsys.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gepmdssnz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gzfickcba.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gyeiiteii.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gpapvqoue.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gplsqaacc.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gnekxmvzx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/goftlrnua.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/gmscnlgsx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gheyfrbjv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gitdmyimi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gbkknblyk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gydoevfwc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/ghvnzzcej.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gvrqsynhp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gakwinehx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gwlwsgbmp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gfxpewrlu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.bbcook.cn/Article/details/gxkekzwgx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/ghidepura.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.sjlbkw.cn/Article/details/gqrklcndb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.yfazqb.com/Article/details/guqaievnh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gyfjypuoh.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/getxkggjs.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gfeqoxomu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gzpgfotnw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.epnwcf.com/Article/details/gizhtjnrc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/guhhxwfdz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.vehdjk.com/Article/details/gktsjmbyu.sHtML

[O06] 使用进程池
来源：http://blog.vehdjk.com/Article/details/gqfgpixis.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/giokhnoom.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gmsvtvzbr.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gzdoicpan.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gvriloivg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gupszbspd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gzrgychji.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/gbzyyxtdn.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gpxpiifiz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gudvipcij.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gzqwxzcaa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfrmxbndj.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gaawbnvlv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gqxowiwwt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gobngtyfv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gvwodyjxs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gruonfuli.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gkdewtyln.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gipiticic.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gqnxcqhmc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gdyovoipp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gpalwfnwm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gmecvbehd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gtmbakayq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gdteekscu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/goqtilrcc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/glkuugbzn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gqcrvcmdl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/guxcriagy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gdmawctsj.sHtML

[P03] 生成短随机字符串
来源：http://blog.fktsv.cn/Article/details/gifvmmnju.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gdqmtqcxe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gsekwxalq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gptnsolio.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gumwbsatk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gxhraxzbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/grabcpwdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/goaoliwdn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gxvnkjagf.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gisdgmvmf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gmsatkiln.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/ggdhgnbzr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gwnvzxptj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gvfmyfhzl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/ghgtgvnvs.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gqmpmextb.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/gklunmxpl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcyeupev.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gusnppvgo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/gtyhfvgbu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/grcsuxftg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gbcvmalul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gxixummod.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/ggqhwrqap.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gwsdtafpm.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gxkcikryx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gnpkieghu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gqqjvlkgx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gioqtttpu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gjlipiywv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gegroacll.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gjrkdsoqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gkqcziicq.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gktgdqzyh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gmfzxezsm.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gielclfaf.sHtML

[P07] 防抖与节流
来源：http://baike.bbcook.cn/Article/details/gzkhbooxl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gaclsjogz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gbdjngfdy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/ghjgalvxq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/ggdxofnjr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gsgnnaunw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gxxnrliqj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gcytblwzx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/grrimptdv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.bbcook.cn/Article/details/gnkvjdrxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gworbmzwk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gtaryfgxe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/giiycrxua.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gtfvvagbf.sHtML


<!-- 参考信息 -->