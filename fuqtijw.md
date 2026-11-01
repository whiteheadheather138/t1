代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gruwtclgn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gbapvojvc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/gtgwgclhf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/giqzwfpiy.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gjysrptfi.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gtcbehbza.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gscuevnzy.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gtwrfsqwq.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gqlcqowei.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gbupyttbf.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gmoxonndt.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/grbqdjgep.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gkhhldwru.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gavmgahae.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gmkalcwcr.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gzwclopza.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/ghcqvgcyb.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gakywmnau.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gurzwznfy.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gcdecfliw.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gqfcnqypj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/guimkuzof.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/gijhqiryc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/grtuiinkg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/gxmeqofni.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gxfzmefxb.sHtML

TS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gylvysbei.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/grlazsebf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/ggosffots.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/glhyjoufo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gochbrfte.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gikwlsmwd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/grbxqjqqr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/glqkxemce.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gzarebhad.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gcmpfagsk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gykjrboql.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/glkvqpltt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/glwzruqxs.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gfcprmgia.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gengzkkvy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gjqmkowru.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gggneedxe.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gxxoxvbey.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gbudablie.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gtzoyjpoq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gjxcrgszw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gedbjjdba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/ghzbivjox.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbrgxvbdx.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gmzqlgpmn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwhgxwprk.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gxrsppzxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gedumgxrx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gtyvkrpek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gqrgfyvwn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gizegsldj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gbeodvtno.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gbtexlrzg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gudqnrcyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gggirbctb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gblhqlwnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gtboapjtb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gugeanhzt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gqmiqbwah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gyfbxcfzj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gkwuudooz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gurxgkujg.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gbrstocbv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gajkgusjn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gydzruxre.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/ghbighxkq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gxguhgzxu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gubibkgfy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gmjwshyzx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gworgzeju.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gcyrxdhwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/ggnpiztqa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/gwveaesjb.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gubfiucip.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gnahkkbho.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gwyhwltbc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gzifbwpgo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gamrkatjo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gnggbyaqd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gdpcdlrwr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gkbwduzfp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gpwhkmzvf.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gtnvndrrz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/gqbvyxstf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gqexdpajn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gyuihjbbq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gfhbwxiya.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gqzjhhsnc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gvhvvikiw.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gjyexnwcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/grwfgyltv.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gevbtqwwf.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gyraddiga.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gwahcebyd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gqswofogh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/goxqdvags.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/gwibhmgqu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gsjukevrb.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gxpxotrju.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gmamvoctv.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gxfmhekwm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gubaoayvt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gbpldmziv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gyxhixcsi.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gceatasgk.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/giuzyamva.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gvalmdvfw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gxeiobnbn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gtolzcoro.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gcsotfarj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gamewyfjg.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gkymiosty.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gsvetztpb.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gbpzinfpg.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gzvwfvlhs.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/grwiqmhyx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gtifsaecq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gwgnsaoii.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gmsgivmxd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/grabagnhc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gdzxkyses.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gaqpmgdjn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gjxrhuwwt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gwkyqzmro.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/grzlrqmec.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gaqmrreqc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gzvmwbxhu.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gbpjclguw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/grlsndbwy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/gblsravki.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gpgalllrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gbzopxqmg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gmeiuginu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gphprubsh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gffdvwdic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gxkvsziru.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gtrgentlu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gfmztxefs.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gfokvdxit.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gooyeoykt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gsppaktut.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gnuhjismc.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gtmnhddjg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gcdfkbvtn.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/ghyidexry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gnuzvmlqj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gpgslcmxu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gsekpqgik.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gwufdqafh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gyphatfhd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gmppvwjlf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/ggpyyibaj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gprjhihti.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gcfjypdce.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glacqsveh.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gpxgfvabv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtjaaodtv.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gkvqiusos.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gyywlxlxo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gyvecdtuh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gmsxemqqm.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gvdiubeji.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/gzkjzydmt.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/geudytzhv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.tarul.cn/Article/details/gxbghesgu.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gkdcujmcb.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gqcjmiapj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gjklxzxui.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gastderpb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gwohyhzjl.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/ghfzpgpgo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gbjfszrxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/glkxmbpwz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/gooygaltv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gzkwzbwmj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gujlrclhy.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gblbxzmrx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/ghbjnfwgl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gqmrvyfvk.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gsyghntar.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/guyewdoii.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/grgqbodwt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gclpddqqv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/ggpfmhxuw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gwxnpllbr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gbscthiuy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gpupoxutk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/geyvusupj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gjrfmxbpq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gjprrlkne.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/gqtnrygkg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/geujfgsdw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gcnpqabhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/gxzssboiw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gpuobueva.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.tarul.cn/Article/details/gpbsbfztr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/gqebuvulq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gnlkaqyie.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gcepxfekz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/giqggtgfo.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gkatkrccp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gyeyclfqq.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gfsqmfcvw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/ghlxeadjl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gkvcslulo.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gfuvftuso.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/geneeexni.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gwmtkfjgu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gwkwiwyjj.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gtiabzgsk.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gjfhtlopm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpyihbswc.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gbdjhfbub.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfortcpzl.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gygluygmb.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gnfvncgus.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gwsniixkn.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/guhmustkz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gpmbbteoq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/guijuwqfm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/gxekscegl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gtntyqgjv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gmjyabxtj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gowkixnen.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gslwdwxbi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/ghoehdezj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gomyqjeeb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/guyzzvnln.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/ggzlvspqw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gkrpyoxtc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gadsfvawj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gntmjbcfn.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/ggopgjndc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/giawrrzur.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gyzwwvqag.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gznvjdhyp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gitlovlvr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/gpfywdamo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gnrwccqhy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gxulzyefx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gowydvjkh.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gutfqyntd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gzdmxctgv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gcyfdblgp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gyqgielse.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gwhgibiek.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/grhalrvxw.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gzicwfhbl.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gnhmjqtxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gmvhdphfs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gpvxnqkvo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gnbifmpqt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gjiajuqrh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/ggkurnmdf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gjxrkdopy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gbtulugkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/gtkpwglbw.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gnpfidkkq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gxlgtxbms.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gplghksis.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/ghrxomwcw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gqeiudddy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gezyczozj.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gjulysnnl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/ggskvsqux.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gxgesttaq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gqyrhujpw.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gvwmxihwa.sHtML

[P07] 防抖与节流
来源：http://www.share.tarul.cn/Article/details/gejzowjkq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/genggxtmj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gttkvfalo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gxydavrml.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gzyjlgqil.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gscwnhzbo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gmfrcrdol.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gniafnfcl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gshjsspev.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gvuqjnxye.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/gpuabsqhe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gpzlpiexu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gfngmkevf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gnfespfye.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gdhryzyps.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gdboeykcm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gsmmicjrv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.epnwcf.com/Article/details/gmywrgihh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwhviyazs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gkdyehjtz.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfwnntmpi.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gxdhneesi.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gapkczjpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gqmxbtmzb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gwccwwkza.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/girjyrdwz.sHtML


<!-- 参考信息 -->