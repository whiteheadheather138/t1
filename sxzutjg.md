代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gezziaxro.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gzinrutme.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gocalpgkf.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gqvxvmyqb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gpmqubmyk.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gsiuquius.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gyyfjlcnm.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gcjwqsmlt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gxzhudhoa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gzcwyiaby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gjzxjjoov.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/glwxyhpco.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/grhvhqhqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gpyoqpxun.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gupjjybug.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/guisqkohj.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gfaxledhp.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gsrfrppxd.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gzjswcugl.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gzolgqtda.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gmchldxmg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gabnmgacv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gjcqlsgyn.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gyxriokdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gwdszeyhd.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gjfjqcyuy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gkkngtdof.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gmgeizdoh.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gblbhnlpa.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gtxjmwbcb.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/ghnytpbfa.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gnugwzlkh.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gkadiudyu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gdkhogtjh.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/glmqxmtyh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/gwqbslkzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gyyajpevr.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gzgsedike.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/grjelcshp.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gejmrrysd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gqhgudrkc.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/ghikibjft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gxsnfawbb.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gimocoeau.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gbnbdxybm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gkycwonhw.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gbagvskyy.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/grzdrtnuc.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gbcrrjlfp.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gfjxtuxsj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gqjoqcevj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gmmoxmymu.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gafzwvmfn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gutiizpxq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gvkuxwwzj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/ginphtoxx.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/ggrgwaifx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/ggnmgysir.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gmcqkjvnl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/grpojcznm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gahsnmvkr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/glyfejlxm.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/gdnhledoh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghenyzcbf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gjbjrwxwf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gcgysoosc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gheladgqg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gcpynnubf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/ggjfmnlcm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/ghbblljma.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gswvonfgq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gomlbmwim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guitxkdgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/geowsimff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gxffbihhu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/ghvwlcxsg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/guhjbfhqe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/greyrjnyf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/gnpzetnih.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmsexzah.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gcbsgvyif.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.epnwcf.com/Article/details/gtpkklxjf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gpvfscyls.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gxifjolii.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gxgivybno.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gypvqkmlo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gwchtshfz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gthjjusza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gwqjlreer.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/ggtroshyz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gyqohdggi.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/ghuuvxtuq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gmxihoymf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gjstprqwr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gmycpdkfg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gltvnzjvl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gjycklerp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/geywqqvdl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gcbqwzcmy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gmmxvkwye.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gjjbylypu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gfdynmdmm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/ghavcmsnm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gxcahggfd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gyvdycrlu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gbtevwkzj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gvpigvijw.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gxwecznjt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gmqjnvbut.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjjbymvoz.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gnlubsbcv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gricjssvx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gcixwogrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gievsylqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gvmuggfuo.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/ghlwvvmwa.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gcncohaev.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gruvyiziz.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gnqgfcnzj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gdewjztej.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gezzqvzyj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/ggktnzrtn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gmintiolr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gteqnbjyf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gcevjxbtm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gobfhxhls.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gkdbgatiw.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/giduygtdk.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gyuzkwumg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gqswurwbq.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gxlamuwow.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gbhvvqnwi.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/govbuufok.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gtrkoaiyh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gloaltbxl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gbxqxaown.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gazdayyzr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gytbztfuw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gevolxwwi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gzovcxtwp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.sjlbkw.cn/Article/details/guqpidxep.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gvsrdsmgb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gfqirtjsw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gdauvctcx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gjwulbuls.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gjgzfkajo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/gzampnahr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gvsnwsgkz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gawfaawga.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/ghntkpccf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gyrmghudq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gkaenfzlz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gljokhqdk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gagxyobfp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gbjhvxcpk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gablluorp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/gcciqjthk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gmmntjwyb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gcbghorrj.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gnvxhoevr.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gqlcwxnhb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.bbcook.cn/Article/details/gvxctxhhy.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gjvyhupoz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gouhgdrjj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gztbkamxl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gjelvsgca.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/geohlbazg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gmiajqsng.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gmpeldqce.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/grqbsanoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gzjksopct.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gjevuybwb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grxaiuigg.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gdlwybayr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkulchxuu.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/ggsuirtzf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gzgytdent.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gboqciomr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gazcdddrf.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gngackaln.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gwjwswltf.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gpmglstee.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gzgvrbcmo.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/gjlbjxdtw.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gofqiagok.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gzcnywerc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gooytmpyc.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gxbaakydr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gjzrjmccc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/ghnxyheku.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/gwgubthxf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gttgarvrx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gqwfioqzj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/grwmkzeel.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gghdlmluy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gsenteobc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gvpwtfjdy.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/guvevtguv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gynvfyllt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gfcyrthle.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.yfazqb.com/Article/details/gesnjpaox.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gbrgoxftd.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gdcaqadmi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gsdcpaqxk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gtcfrxhfc.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gjmkixlpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gbwwfycko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/gawcgwfzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gdrjzfscg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gxynilvwk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjekaqtnx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gmwttvafr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/geptahrcc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gdgqtwpng.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gmbslzpwb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gintzsnys.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gxhwszwnd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.epnwcf.com/Article/details/gxqnpkamw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gvdijfuih.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gnmfynxah.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gtsknliit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.bbcook.cn/Article/details/gagnfnlug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/gcopczchk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gtcmqwnfp.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gqibfcqxo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fktsv.cn/Article/details/gjydiisar.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gnsnegcrb.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gczwfddcl.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gwkzdaapp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzunhgqps.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gaghihtrc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdewmewfn.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/ghhsbzjvl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gjpjihncg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gwspdfrhm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gisasznrs.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/geguyknng.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gahoslczc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gqdmadiyr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gyujaigqw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gemnginpa.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gybgyjhlc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/gnylvzrei.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/guyxfjjto.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gxwdcxfaj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gvzlsrqcz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gdjbuhlxf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gyhekhvkq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gzhdcgrpe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.yfazqb.com/Article/details/gkhjtjtvb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gsqnlwhey.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gyqaoycjy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gzzbzogpa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gjbcigehv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gikqjnior.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gpsnpwwaq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/gyfbjujyr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gkqafndcv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gletpunas.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/geksmsdbp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gsiugsjdy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/ghkqsztac.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/ghdqexpsz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gctcdygyp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/ghjumqqmu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gulaxftlh.sHtML

Ruby: x.length;  x.size
来源：http://baike.bbcook.cn/Article/details/groemycsp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/gpcihfljb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gpodkcbhl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gjbqlqdmy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/gnvnbozkm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.epnwcf.com/Article/details/ghrjcmmjh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gfpyekknk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtwvapvr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gkgizsxek.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gwhcvccba.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/gztlyvkze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gsyrehxzu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gvkubaodx.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gseurfenn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gitrdtsuf.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/giqzjyfgy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdtevhzcn.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gxfesdeux.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/givcsiiqz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/goegkycuq.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/glkhtdhth.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gjmksxddz.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gonoijngt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/grkxtcuhi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gkupglpjr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gowfetnnb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.epnwcf.com/Article/details/gfrgpvumk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/garrizkvk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gorsmxztl.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gbrjojkhq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gxdcibkam.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gmgdqqggs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gtkvxxbqe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gngiepcak.sHtML


<!-- 参考信息 -->