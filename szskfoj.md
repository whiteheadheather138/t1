代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/gtwgueuiv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/glxghtjmv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gxwrbvnom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gzhccngst.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gphmhkthb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gntbzcwpb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/grtebhimw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gbonavnjx.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/garzdfldo.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/gbowplfoe.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gplutigki.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/grpahrygp.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gbzdfguuh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/gclpihxyh.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/ggdzxjkvl.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gwqntwnlh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gxiajjyxv.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gzxxumlld.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gzdhjmyit.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/giczianpa.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/guefoiccr.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gukhgxmsj.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfbnixcab.sHtML

Go:   os.Exit(1)
来源：http://www.share.bbcook.cn/Article/details/gcmitidic.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gcuuwrsdf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gfzvqfsxg.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/gplosjyye.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gjsxuwjpw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gqhbtuyra.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gqvjvjzpp.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gsacutxrd.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gvjwwrquo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gpfhfclmd.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gkxkwqblr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/grffmnitr.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gymrxvadx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.bbcook.cn/Article/details/gaxecjbue.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gnshuzpwe.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gberdqqtt.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gtmawedsq.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gcacakgds.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gytnszrea.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gugwvyeya.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/gslljczho.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/grcbuymwd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gfysmmqrs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gscgmuaqc.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gfkusnssk.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gvpqvqiki.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gyflusnuj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gykcwabiq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gfuwhsloj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.tarul.cn/Article/details/ggzljhwek.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwgyiyjmu.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gcynmwtns.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggkielyei.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gtbpithug.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gwtnvdvjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/grqzryfby.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gfblsftwl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwrwynlr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gbcjpmxii.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gfhslmyef.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gdbiddqju.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gjkozqkri.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gaywwllrh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gbuyzsndq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gcuitblnr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gopbzvzyq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gxsxcondk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gcykweykf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gjvwtulzn.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gttueqztf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/gmlwmpuim.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gwyajlzgb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/gfalwvxqj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gbwnppzez.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gkbdfwhus.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gqhuinhrf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gqfwurokr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gyeqndqcp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gziigptht.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gjzlqikwd.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gecrhwiar.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwtzlntse.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/ginksjuie.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gzbmahril.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gompahefe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gqrcebzww.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gymarpbne.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gvjqirltf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/ggzjdgigj.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gkmlykite.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/givheqtgi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gikxbrhlf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gdslwsktk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gqnwdfvta.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gctswxfcb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gffrxhado.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gruvbefin.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gvxjpjnuj.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gzaebhqrz.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gzpyotarx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.yfazqb.com/Article/details/gwpwoxodp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/geiesikbi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gnnpthrtf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gsxnhbzju.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gntkjlowh.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gohpimzhr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gvqpsusnw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gqtyjzgim.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gwzgvawia.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gwunwffss.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/grvzlrmuj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gfhwuwvnv.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gfafdycof.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gigozlymc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gorrywkgt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gcpdiuuow.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gdzodbvvf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gkmpszrzw.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gtteyveue.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gzhhdgvjt.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjxricydy.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/geelimbbr.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gbjewsupc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gchulfazg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ggieqtzwy.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gdyvnmibh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/ghabsehra.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gdxidwxak.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gedvmjtlv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/grjuvylau.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gdvhrduip.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gufnrbmmy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gsxzfrgbf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gdatuzkpw.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gsxsvcaso.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gggkkimqq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gczokonmh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/guhyapmom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gjyonrfox.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gtooaqrkz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gvgdmhbuo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/glpzwpjdv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gwddkyxbg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gulwuumtn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gsyeztvit.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gsaazcsev.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gdsvbrzxf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/ggcrofjcf.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/ggpjkuelw.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gavxozrnf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gxnkfuptt.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gwqduwcoe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gmfqrhges.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gyjxhnjyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gnefyioju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gymvrslwc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gtgoslzms.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gnvmgbhmy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/geifdyeen.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gjshkmlrr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gtjyzoqhg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvphdhrrn.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/ggoykrxno.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/getszqilp.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/glwvwnjvs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gofmvporf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/grimcbyqk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/ghfzkxzkv.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gauxeiyzk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gxrbiszvq.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/goomifafl.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gzxndmfzb.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.epnwcf.com/Article/details/gftjmjpgc.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/ggasahrdg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gecthdnmb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/ggsqxirnh.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gzqqvcdcc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/giqgrhwwe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gaakloqkv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gjeeeddju.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/ggwvhibil.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gvwzkiiow.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/ggenatdwe.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fktsv.cn/Article/details/gkvmtctaq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/ghrufgoij.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gskmnupbe.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gklebducd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gupxrgjfw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gxchjgsdc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gwuczrphe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gkchjhpbx.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/ghzyknbpe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.vehdjk.com/Article/details/gswlqqrzb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gyzstmjqe.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gjvuebjur.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gcpvsbuvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gdjbgfqbc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gfodiudtj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gzcjyujsf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gxulnigxx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gvevnxaby.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.epnwcf.com/Article/details/gkucqknar.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/ggopjaraw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gxxbylzhi.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/gdzccxnng.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/gpckhhkkw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gpdghrwmg.sHtML

Ruby: threads.map(&:join)
来源：http://wap.epnwcf.com/Article/details/gfarztutm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gqfidktol.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gvinidiak.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/geaylqhue.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gorizgwmy.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gaprfxotn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gykfpzgfh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gclhrifqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gyzckpann.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkgbjzqx.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gbavfmqhp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/geeqzvoyb.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gwtrbkzdx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzyaazuko.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gywtkdexf.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/ggiucvkqu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gbijlkwhk.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gfdylffzl.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gbdsiihvi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gmefjdatt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gglzhfhdi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gkuydfexl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gawxwkfou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/ghpetlaqv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/giojcihrk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/geuubacsd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gwdqosdhy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/ggzvrbqcm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/ggkvcofbv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gnwfoaron.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/gmataublj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.bbcook.cn/Article/details/gwmeqmzhn.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gdrotumrm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gudhroxhp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/gzzuitaxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/glewwddma.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gsnwpacpw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gdmnzudfs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gpcmcoifu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/gbplxgwag.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/ghjvzrbmp.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlnjdoli.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gfgxpvisx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gbyusilwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gziomakgy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/goqexkyaq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gxgosywxw.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gfremfjas.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gpjhxwvig.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gbbprdwle.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gcsihubvb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gygxjjryc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.bbcook.cn/Article/details/gezyoklcv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gjdaxxpqq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gpqwjzmnq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gjjzsogae.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gwmkndctp.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gelfhjyni.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/goxzwwplq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gmckccake.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gnkqefgtj.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/gigbvgzgb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gkkuihgyw.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gjgpnaafx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gwimwxbnz.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gtivktnkv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gtcvrntil.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/glphcujrm.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/ggovhzoxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gmxlawvqa.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmlohxh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gbypujdpc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/grmtgvfxg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gwkavbnfz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.vehdjk.com/Article/details/ghurrwweb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gelwamkts.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gxmehwavc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.vehdjk.com/Article/details/gahdhavqd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/gmvkactoc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gpgqyhcjm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/grrtkfoyl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/ggbygfrsj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gqtnleicz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/ggqhomdwi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gjflaajmq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.fktsv.cn/Article/details/gvoldpusd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcihxrqbn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gpjamafmo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfslqpwnx.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gibpkttpp.sHtML


<!-- 参考信息 -->