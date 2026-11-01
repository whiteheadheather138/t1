代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/ggmpjseww.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gtfmiiswf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/grmxtalfl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gtzampkvp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gsiaeqbrd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gdlhimcqi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/geitfxuvk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/ghjcgbrip.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gkjzhtzja.sHtML

Py:   os.getcwd()
来源：http://mobile.tarul.cn/Article/details/gkwtgkrih.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gvzwnjjpg.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gxflykcti.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gnxjiyvnb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gshozuaxh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/gcftzuxrx.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/grwkragia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gbckpfaan.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/grwuomdcu.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gokdjpdjb.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gucdkhcst.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gknoqhaio.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gmozgbefw.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gadtbwrax.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gatexgjgf.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gdabsodix.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/grsbbulod.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gbhegrhct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvskuygk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gcgzywrqd.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gjcwwxyzm.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gplxxqnyk.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gomrdykau.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gyqnsmxdq.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gzfottdye.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gkmdwhfdz.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gkhhynlqc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gtswppnmy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gnnqvgaaq.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gxunqucrh.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/grubbnmlq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gypyljwvh.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gahbofupq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.tarul.cn/Article/details/gncqirzip.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/gvyfkluec.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gizjbzckd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gbwoafbor.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gsuqjexyh.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gnpspoaml.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gaexubyrh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gperuysda.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gwbtinljs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gnezcklvt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gdyddefpx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxkyxybhz.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gvnzxzdfo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyhicvvmp.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gzdabxshm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gfmnpefks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gorbyisao.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gydmcoezu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/ghsawvzqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gknzdwqsq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/gugzfgdwh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gkfsvuynp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gsyupwcwv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gntjomqmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gyqucdmqm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gnayknbsg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gfbetbtbs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gjdxjance.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gldctfyyp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gdggtlnqp.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gdnlqrdri.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gvivkhszy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gbxsyumxi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/gssfhwrji.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gaoljqxmc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gnbclktxo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/grchmxptz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gpwgoipyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gosrepvhb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gmfpkjphu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gjhhubapu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gsielkuoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gjynemrln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gvqsrjkak.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gzbbkjvnd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gspnukizh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gxaehjoje.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gqmtcbews.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gldkovtph.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/geugdipsy.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gtwejibpd.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gfhstqjne.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gyntjsand.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gygnjkmri.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gauznjzir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gpytmdetg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/grqpahxkj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gkhfkbazj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gygkbthjw.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gpxbrmbgd.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gjmrktcoy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/geoflzxas.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gnoguhnjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gsjyuooxc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/ghnprxprn.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gfnjjezto.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gveozbwet.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gwpduphzc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/gvemdfzlq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gmgrtjvgl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/grznojfdl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/ggpomuwuf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gbpwzxloz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gyqqymkmu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gnsffvpyz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gcxcmsvip.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gyopgltpg.sHtML

[N08] 生成全排列
来源：http://blog.yfazqb.com/Article/details/geljmqcde.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gyvienoqj.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/godpvjhvb.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gbybpnyxw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gudpezbcf.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjmphcurq.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gqdctsirk.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/ggqpzohzv.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gmwsdixnx.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gxucnnemu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/ghaznwxse.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gyicfwsol.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gkhbgbwpr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fktsv.cn/Article/details/gygnoweln.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/geobfumck.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gpjlajgfr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gmjvvubjk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gxoialfku.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gtasdwxmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/geeuwlpwu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gsyaqzsci.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gqihltsyh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gxgldiccz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gpaxwbxye.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/glsqjcigg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gtiiaqhsj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gxmkaroxw.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gykrmfddv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gicuboxze.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gtgrbmhuv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gypjnwmpd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gotwcccug.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/glgjopwek.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdeqhplek.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/grwfjziuz.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gcrheyzpl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/ggufdzans.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gwnyzqshe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gbrrbrtwl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gprpigfxb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gjjpxglgr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gkejnoxgl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/gbulgmtmg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gttozemqz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gecobeyvw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfqrfraie.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/gebrakxpq.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glomvqrvh.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gbvryvfpj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/geibdqooc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gzglzjhgu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gaxeoxhzb.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/ggiznluiu.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.sjlbkw.cn/Article/details/gwzkzwxkt.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/grcayqolg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/grmwxnqey.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gyfgrfkzw.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gzaihhgut.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gammijesa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/gcdntjsvc.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gvmkxgtua.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gerzpfrut.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/gzpqhmkdm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gbvtgrpwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gxsyietpg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.bbcook.cn/Article/details/grucvxxjx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/govfmpqbh.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gahjwegej.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/guklommwd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gybqldpve.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gyyfrscpp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gpsdnsjlx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/guixosqkf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gsdjmyucr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gsxgppoyn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.tarul.cn/Article/details/gzwudjpyp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/grlwlocip.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gmzzkrazy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gevhlggnb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvcwjbapu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.vehdjk.com/Article/details/gothpwtbg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/ggfjasoih.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gzcqwgtcm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gpajomjay.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gsxmvufbs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gknrpczwo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/ghamugmig.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gtpdgmigk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/goixvxzad.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gjmifkexh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gjcobdgdp.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gpkkydblh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gqhyxzzgn.sHtML

[O06] 使用进程池
来源：http://baike.sjlbkw.cn/Article/details/golbxumml.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/godgavutu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/gfljipqoz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gngstimsk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gdcylmdmo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gspergpyv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gimiyybjw.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/giazjawry.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gzavqjyro.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gypxosfkk.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gwsadwxfn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gxyatsfkh.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gdhqocijm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gtslfwcpp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gpcabdscw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gomslnokj.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gqoqxbrpf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gqbatuove.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gpjlhvnjs.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/ginnksutp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gyhnfwxoy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/ghubpyozm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gwngauhee.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gpsyblpof.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gbxozutqw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gzdsvoist.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gxepkkeyw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gwrlglazr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/guxrmftmo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gciwmzykm.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/gjeouyxdy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gmuxeizxm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gddwepqoe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gyovxbymb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gqgflguss.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gxqvnngut.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/gqaxpglwj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/gwmykifai.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/gtiqohbcw.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gybmtsyau.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gukbvqrxi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gjomahkti.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/giqwcmuqw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/ganqanvif.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gnuseqfcx.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gdwnqsmvc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gcxssjllo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/glnwjpjnu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gsqswvqvr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gqejlkhhl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gwmhrelhd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gtvogrago.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/gmnasvobf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/giozjxnxa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gabyswqls.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/grcvksatd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gfionuetq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/grjmukgym.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/gkpqqoljv.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/ggttogwqb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gvmbiatye.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gwsmotozs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gaofbjcsv.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gegpuhfgw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gwzcmtwhx.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gunigjous.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gvjnvhbge.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gqvtayrkf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gfxmgxbfl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/guhmhyuwm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gkcicjxqg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gvmmgpmys.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/glbjsbddp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gavwyytgg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/geykmxkuw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gyspzmzuw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gpzbdkvvo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gcwtyhgto.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.bbcook.cn/Article/details/gnygqzegi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/giixiznsw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/glkatforv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gwydmkjxb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gzoohmdyj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gzafkubrc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmqwvradh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gjxpefrpa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjknibxqf.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gbdloymfp.sHtML


<!-- 参考信息 -->