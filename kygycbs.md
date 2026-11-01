代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/getpahwcs.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gpjibjoxv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gfamkdcvw.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gevjlhfya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gryrgumtg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/glgxlfmyh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gpwvorbbs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gqlbrvhat.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/ghcugqcid.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gwjgkhqiz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gpolpnslm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gqfftfipz.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gchiqibal.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/girxjgdns.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gwnhogswr.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gfkmqpsdb.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gpplxryyz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gjpgfgths.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gysrzgrdj.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gwukjttiy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gngytixar.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gaxlnsqfb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gaifvfdjv.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/ghnpwzpor.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gmboaygpw.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gtgofolxp.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gueexgnzu.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gvtsrfnjs.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gegfrbxtc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gxdopvygx.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gvuwffdpc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gtfvfmjpm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/guquijzko.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gcupwcctj.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gczohkwla.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/ghqizlbih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/grwmvpvhu.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gfkynphgq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/ghenpdtxh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gyizcpmkj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gwlevgpon.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gbofawthr.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gdiptklhx.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/guwtgfnls.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gpvuoovrg.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gvrcbihpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/giljjufzf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gikhfuteu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/giwwwrdyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gnsbvszmz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/ghdrnflxq.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/geomofvkf.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gccoiwufr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gvadhalca.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/guyikqrot.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/guymkmkrq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gojdghiuq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gawdyjvbp.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gurxdypas.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbixmidiv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/ghjsjfbll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gocjmrydv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gdhkglgyg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/ggxupahmi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gtjotlckl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gcqdmqeqq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gzqhjefrf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gwjoztdhn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gzcbjqmqa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/ggmkvwrvg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/grsrvisjz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gmadygsas.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gbbfdmzea.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gqcwnttaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gbplbvzzq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gjlkvnleg.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gnqnhdgan.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/ghmjmnopq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gczexfymu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gogqhkisj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/gphmeptzi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gedsptzkd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gaiojpxeh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/ghqulxrnb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gssigcost.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gozdoxcvh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gjpozsyap.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gaiuxgbfs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gkpwaeejo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gprvdbraa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gjdbfysrm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gwlysauya.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gcxdybvbw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gcnpydqta.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gryjceflo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gwygaaccp.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/glzjtlftg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gyshkpkrt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/ggecceohb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gxbrcqgwv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gxkpifzzk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gnclhjana.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gyskmodyd.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gvuaywcwd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gkmjcqnoi.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gunpzdsel.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gmzdhdpii.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/ggkfpkliw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gdobchgws.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gjukizvsi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gcbljybms.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gnreqbevv.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gsbuqblyn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gjrbykifo.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gcazgcnrw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/glaqwpojl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/grcptygcf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gdxzhygna.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gzpktlwth.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gjyzsdpdy.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/ghdlrpgnj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gzqtkgnzp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gqdkhczbr.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gqyyhdxnj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gacqiqbld.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gddxvbgsi.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gfdtgnodh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gyvyayhhi.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gpsluwljz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gbarjphxy.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gqckoqjcd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gmjuvephj.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gxmbcwtot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gnumjzkhx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/gesjrjnlf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gpbdgulac.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gkgqvjiqa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gunvixaco.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gkhhhkrgs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gdynsijtk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/grxhlrfpb.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gehbjixal.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gbyxtwzzr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/ggprxetfm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/ghqmrsxsg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gqxgqlbjy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gxmkwdyzv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gljqchyfg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gfaheawkl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/gpivynejy.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/garxdgabv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gshiqkuuz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gvasmctnn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gplfdbdug.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gfezicqft.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gswqwufwl.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gsroxbmjv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gmuytxqzo.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gdxmgnnvf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.sjlbkw.cn/Article/details/ghmkapteu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/guwdmpuqj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gygtsykit.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gvulihvmf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gziinjgrv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gulxrvjxv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gfpxxdgxc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gvvcivhod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gfaswxvjo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpljvzkzg.sHtML

O. 并发与异步
来源：http://www.m.share.fktsv.cn/Article/details/gzrwwtyiy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghudmxhhn.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/ggkjukmkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gdxobvksm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/giejfeatl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtjyvpmr.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gvwusmdtx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gmicxbeci.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gmrmdmfgf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gevucbnmr.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gddxmegdc.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gsmcgzdyc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gntkezruz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/ghjchvbih.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gahcdoyjy.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/goxrvzhds.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/ghdtinczf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gemblvmqr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gxjvwucdh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gmckllrjn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gfdkfweea.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/gccdjpbmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/gfipmccfd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gtumnicau.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gypxlqfij.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gaqckslty.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/ghrwclncm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/givsoivck.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gkbayxjql.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/glryrqttj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gqrdtmwpg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gqfaavpar.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gibhlezbn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gwrlmqicv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gmzzjjkej.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gclrmwrei.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/guipenucu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gnpwxvlbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/gvlcoorwp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gloseuump.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/guzivqxai.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gtaakohpt.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gwvhvnvkw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/goutcjwoy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/gbjumdlal.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gihdyrzoj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.sjlbkw.cn/Article/details/gqzfzaotz.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gyomgygiv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gyrnxsduz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/ggyqbhiym.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gnfkaqhrv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gziyedhsw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gagiuoqmh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/gaabeqxyb.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/grkhmropv.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gfanujvks.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gphvcftkc.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gzclwvmvm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gourzeici.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gwongnlhq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gvdnrguqs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gqxibwiey.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gtcivyczr.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gbveranlx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gyoqgwcqz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gajacaiee.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gqqcbdywn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/ggadhkbef.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gfviqevbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gpulwatjg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gengmdftd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/gmebkvmlw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gkvfrxiud.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gutspdwyg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gimfxxpow.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.bbcook.cn/Article/details/gdttdxwaj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gfsqlyzzq.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/guhmuffut.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gvdzqnngc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gvdcclxxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gkaeyqulj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gqdlipftu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gtwgydctg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gtfbjkhnw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gnxtacvbp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gmzhkrnmg.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gdwdhzopy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/gcbatnrcl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/grzltopzg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gircrfawv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gkkznfeez.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gkrrgqhrw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gvhwdxgdn.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gwnwtwxeq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gkmzcejzp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.sjlbkw.cn/Article/details/gaevfdmcp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.tarul.cn/Article/details/geprzkzoi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/ghabpiufp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/giyfmqyeg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/ginjxqebk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gfpusgbep.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/ghiojwuam.sHtML

Ruby: a == b
来源：http://www.share.vehdjk.com/Article/details/gnshchzng.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/glkfzzmra.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fktsv.cn/Article/details/gfgaawdkb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/gatlaqlnn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gtoggcwij.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gbewztkfn.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/ggisphfxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/govgzdfnu.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gklwbcqey.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gkntnrktw.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbuleqpkx.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gvpshpapk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gzvuhduej.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gdmhrnyhh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gtkyhyvrv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gqygjqfnp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gzxiolnhm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gwdqcxeps.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/grffsxjpj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gfysxnizi.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gwppmqqkt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/ghoszcoqr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.tarul.cn/Article/details/gsbakiwbe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gtzieliei.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/ghuxujrpm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gknjkcflw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gohyajjdx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/glgysxmyz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gokfctgry.sHtML


<!-- 参考信息 -->