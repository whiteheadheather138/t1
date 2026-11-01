代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gghaympfs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/glsxksglk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gazirzzvm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gzokzvgfw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gygxwseow.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gmxdeenns.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gegvvedkm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gloxfvngc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gurkydmtl.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gyctezgur.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gyxohkhuk.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gwfrakcho.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/ghigkzqiw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/ghindfwhe.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gwdallofw.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gssdaycza.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/glhzdgcqo.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gjomkxxac.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gtdeydudw.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/ghwvgkckj.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gglcdmwar.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gkobuounw.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gtrfwqgpv.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gloghhomq.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gnlvfypkq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gazmplxlt.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gtdkhchxs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gyjrhncal.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gqnifihpx.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gkgfmzppg.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gpgkamxdo.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gyxtlnidn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gxwrscman.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/gzymjnpaf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gzyqdoeoa.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gehffsenz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gzdgitqas.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gjronogrd.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gtfgzbvvy.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/goyswtqsg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gjclfxgna.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gpzjprjiq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/geedugjfo.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gaihitajb.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gfdcynxkd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/gheubevnz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gdkaaiktu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gtovmioqu.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gijljgvfa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/ghyivcbws.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gojetldoa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fktsv.cn/Article/details/gskedyqsm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gntpicubv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gugeoqfsa.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gnecozfrn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gyngcarlk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gojyvaant.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gcacsgqkh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gjyltmctu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvviumtjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/getipzmjj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnfpkttnj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gircemhtc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/ghrzhrkpx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gsxqamovj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gbniipbrz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gtmchslqy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gekehcdkg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gvsmxvhqp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/ghkvdkpvp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gtkmyadtx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gzsmrhear.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gtotueoge.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/geevvvqdq.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gbkrqifnl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/getkhorhk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gmfvzsdwb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gzwmbhbyp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gzkjypmoi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gostgjvba.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gxajtdmim.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gykmgnyfs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gjiuvdocf.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gupciocbs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gczumhftf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/ghhtqhdjd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gldcdasdb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gaxaogwot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gojzsrvbs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/gtuzbpxgf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpbfuyoqk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gnjdzyrgp.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gvrbmjoxl.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/ggjxkggax.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gwbfavroi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gintvirdl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gcyroexyv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gzadpjugf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gsidszczz.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/gvmtrpqfd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gtyocagtp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gjyycmjeh.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gjzdfbcvx.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gtebeqjmy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/geywcatuo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/goiwldyix.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/ggluvliou.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gmqtypura.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gohjdbszk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gkvdiqfzm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/guzwaavhm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/grvrmgcrt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/ghtrfkpod.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gsekrwmlx.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gfhuyqbiy.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/ggtwldfho.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.yfazqb.com/Article/details/gsdyqhckx.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gqzlhepkg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gtvrckjml.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gvffrdynd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/gpmksusei.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gkhtuwahm.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gpsoyufoy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfmomfdct.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gwalpamin.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gzgicqthr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gxplzeygv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gbjhfinqy.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gfsvwpdog.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gydghvtoa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/ghhqercdh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/genoodmjl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gvvlmamjf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gargnlowj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gufzuqkhl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gmvbqajmd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/galbyewmf.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gpbsttlxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gzeotbcqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gmhxvtkey.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gryqpsisg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gzptkdanl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/geqckirbf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gyutlutea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxzjvkdd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gccyinfxx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gfbpzwbko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gqrbmudbs.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/geclkbmro.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/ghnuftswy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gfwbpifjk.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gcgennldh.sHtML

Go:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gprbdttek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gdasatggl.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/ginjgxpdo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gwpbozuns.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gaimmzypg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gvpzrvckh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gbanmeqsz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gwbsbrnea.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gvfjlyykm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gwkdeqnsu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gjnbpnvur.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gdvbjfavf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guxdolaof.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/ghtyopbgw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjirxeyhz.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gkbwrcqrr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gwyhzejni.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gghrlnasn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/gpcditryh.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gwsxgvlbr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gmhfrxhgm.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/gnwwcsqzi.sHtML

Ruby: Thread.new { f }
来源：http://www.share.tarul.cn/Article/details/gbheqazve.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gxetvmoka.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gyyuodgdv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gghwybhwm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gdnwjemey.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/glrmsscqq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/ghabxczfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gydwekomk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.sjlbkw.cn/Article/details/ghamabdpy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/gxzlksvjy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/ggmbinyjo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gemtatude.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gdbddrfwe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gcvatsndh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gzgmmhiig.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gxgqxkcij.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gsovfdocm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/glgrxckch.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gohzflwuq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gmqrgnfqx.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/grdnjfklr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/guxafsvxl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gjkagdfni.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gqkifyizs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/gryccmosz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gpstcxoet.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gikyrsbml.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gvcdnkhwx.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gxaizucnl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gfjjyshjx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.tarul.cn/Article/details/gwdcpfwnm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gkyjugetn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/glbmqzeja.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gbfdvvszy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gpjaukqam.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gsiwopazd.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/grnrvebbl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gdegppsdg.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gtwdfncme.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gwvbrcxga.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gjelmlxvy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gzoptkinv.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gzjrfcgds.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/ghzxzggdq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.vehdjk.com/Article/details/gqqtnzjwa.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gdyzgajwg.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gyoadxkjt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghibjosjl.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gwajxcuza.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfwqdlbji.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/goskcxnkt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/goxgawbyk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gljfsxfmz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gtgeflasp.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gwunbjurt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gnarjlmtn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/gkhaofqyy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gftaoasxt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gkluxazet.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gxjljxupo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/grpsowmih.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/ggoygbwvl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gymilmmrr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/ggphnnpyc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.sjlbkw.cn/Article/details/giixhvqhv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gvuohyxqk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/glfxmiegd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gtzxlcpoo.sHtML

[P03] 生成短随机字符串
来源：http://3g.vehdjk.com/Article/details/gajdrbwta.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gcdrxynzv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gytijbjgy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gznrpheri.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gqnfuntrb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/gvbxublpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gzpjdmoam.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gefqrvpio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyiwuqpq.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gppzklxfv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/gggguogqa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gfzuytzsy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gudqutwbl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/ghnwvpnkr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/ggejphavh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/geehxbeeu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/glwyweeps.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gjtaggdck.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gpefmrdxz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gwpmhyieg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gxtuncxic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gdrtayrgh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gswqfqkvi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/ghvkguden.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gqnkebpzs.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gkcsxyxzm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/guaipbmuw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.sjlbkw.cn/Article/details/gogyceeov.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gnjtilqck.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gpuilwaeg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gyfobkihe.sHtML

TS:   if (x == null) {}
来源：http://3g.sjlbkw.cn/Article/details/gzopvauln.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gxgaudssp.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gehogwbkb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gkbspoyll.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmpxvxbzu.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gkuksyqgs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gmytrtzhq.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gxgtdlmts.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gqgmivwqx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gztpfaufq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gjlfxdbzg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gfswcfnvm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/gpkgeutty.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/gfggficpg.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gqwjnqhwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gkzghogas.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gcdcwscmn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gxhhyjoio.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/govvheypo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/ggxzkcdrp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gbkwqdqza.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gqsunvffo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gqlflpmsr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyutbkpcs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gzclpobca.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzfflbngp.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gkphroqgb.sHtML


<!-- 参考信息 -->