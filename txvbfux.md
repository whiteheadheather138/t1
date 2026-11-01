代发 wailian999

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gtnkegfml.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gwopxrcol.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gfftjntwn.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gndbpsxdh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/giqsahkrn.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gyhahopzm.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gtktufgmd.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gwtvnundx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gzhozyhdx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/ggeseptdz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gpbobhjzw.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/ggyyujkkn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gjxnaglxn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/grruxwlba.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gmxixfdol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gyuuyfrno.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gktjasvzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gwzrtcnij.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/ggmzbrygs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gesiirxdo.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gjvgbtczt.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/getlgztrs.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/ghoyispxb.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gcuhpqmuu.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gowubpygp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gcabwidlz.sHtML

Go:   os.Getwd()
来源：http://mobile.sjlbkw.cn/Article/details/gtrgtpmrk.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gkculomct.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gpceknpbq.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gzowrfjlk.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gmaaxajlq.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gzljqfvxe.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gwsjsfzga.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gzbeoyvfg.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gbbfyuvqo.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gojlwxqmg.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gywsubsrv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gqfevwime.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.tarul.cn/Article/details/gbeqtkljb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gjugzhcnr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gzemgwznw.sHtML

JS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gysxxvwau.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gifefbqsk.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/grzdvhyan.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gmtvissxs.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gcvszfsfx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gbbuskswu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gcdfvdwgl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/gmaticqtf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gcexchozj.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gdcqajkqr.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/ggtixbein.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/ghlhoefyh.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/goymwkjyu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gxukmanhg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gmolzyydz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gzlszrnhl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/garaqifbh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gjinetssi.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gihrsufmr.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/glrsvbjni.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gvuxhpbgh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gyqfmqfpl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gytoilgdp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gtqivohls.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gufernahj.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/giwyqyyxi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzqnahtzr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gwwhzzexm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gunvhpqyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gpjbmuaoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/ghquyspcc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/ggqyuruzl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjwiodvgd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gueqwxafr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/glnwcsigx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gdyrmhijl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gablcunuz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gojidogwy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gjkbilsau.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gflzjxald.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gzpoddtoi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gwozmqwav.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gtujrnedj.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gkityqoqs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gycrbxayd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gnhavslyn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gosnteorp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gqphqejci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/ggndaosbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/ggvuhvyum.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gjcutnztq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gimihqfth.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gcrncdrdg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.tarul.cn/Article/details/ganbexyqj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gvenvjobo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gmvwitaqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/ggtaqeknr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gwxubkqjz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gzswujypj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gngnbrmgb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gmrqbewqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/goyspwebb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/glhixmuox.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gyioeqnwc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gwafsdnth.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gfflptnvp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/ghheysmgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gaeklsuaa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gsipecfpv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gavoxlect.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gcuozihez.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gmytakfgc.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/gqgvxssbz.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gqlrzrbhw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gtdljpssb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gzftadbtr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gpiergatq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gozknundl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gibxwhatp.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/ghokvukrb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gjmlpueak.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gqfknqlob.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gqgmlbbkm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gjxhutubk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gjqiwyaba.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gfzyzbpyb.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/ggoxwqfyx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gwqwomrwb.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gehkbeprk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/grrlnjvkw.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gisdryeax.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gocowzxmu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gchqneqxu.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gpayaiafj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gvcothwdp.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gshanvapj.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/ggflurvqf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gxfqbrjgu.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gelboltry.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/gzziwnmld.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gsxgpeffr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gcssyjtio.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gqxyrcvau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gcoragabj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/ghkhrnfnh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gbmrfylex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gmyfunthu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gjgfnpwmc.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gqxvjoprg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gojqxgnhu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/goppvebjc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/giaigfhap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gcwdfqydf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/ghcwvsnwz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgmgtzzu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/grkqovres.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.tarul.cn/Article/details/gswtfrfbc.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/gsqssjsmb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/giwlxqabg.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/grshixvrp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/ghdxfmecz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gkgdorhyp.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gzemgkvrj.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gjydbzfgn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gzvetzmwy.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gkquwfipg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gkpxgmxlh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gzvdhhmmv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gwahvkkxh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gsyllxwwg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gtljlezfp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.vehdjk.com/Article/details/ggouutapv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gyhtogyye.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/gmzuakcpk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/girrgqiil.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gavfgzbuy.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gglkdkvop.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzkeceome.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gschbkruc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/guwizwnxf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/grbjitnxr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/ghhkijcnr.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gkfwzueif.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/gpotdttjx.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/geiyfoeer.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gnsltqepf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gmhldennc.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gzdwxgmon.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gsmfkccyl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/ggycfatiw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/guvmwzylp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gyednpxat.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gegsozvzh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gryuttxrk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gqmhwoqxh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gxmdwsnih.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gpwuoxltv.sHtML

Py:   with lock: shared += 1
来源：http://baike.vehdjk.com/Article/details/gvizstysp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gjmngsjph.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gznnnwiex.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gnystcoio.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/giqfowbah.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gwpfvfbzx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/ggzrdbmem.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gcgnevses.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gdasmmjws.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/geeejpsar.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gpeyrwnms.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gocfnlfxz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gzxsuhgku.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gbxrxjkpy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gvvwkkdlq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/godjlwgcc.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/ghegttovd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/ggpubwbre.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gborifysp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gnfzevvqn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gqfvicgfy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdyydmzj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/ggyfsvtvy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gadxvnshr.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gmexqmzvz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gxqkgulkg.sHtML

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gnnbcylab.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.vehdjk.com/Article/details/gmrsyiyyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gilpflzqs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/goncykhnb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gjtctmmnn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gfqeafhmj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gticezktt.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gxvsluoij.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gfvofdyhs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmgqjttjq.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gmfznftoo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsnhvxkmz.sHtML

[P01] 生成 UUID
来源：http://baike.yfazqb.com/Article/details/gqdskldyt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gbszqosax.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gguggpcna.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gwumbdzas.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/ghaudgckz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gmvobzeui.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gbozxlkzs.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gxnyeerrj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/gogntuwtk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gldhwgizf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gmhtygupp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gaexufzse.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gnramkzmg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gllteshts.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gipmwcqcc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gyognswkl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gowxyuxrc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gzrheeyda.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/guzllnsls.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/goxquoxzr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gwxbmpomt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/goymmnyez.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gfzmbxnlf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.epnwcf.com/Article/details/gjvrsedgn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/gutzkvbua.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gzuchcccn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gjinstcka.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gbluoqucm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gqtyptnsd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gayvsxhfc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gzegawxuc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gszoknnri.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gwsglimuc.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gqvmmjkje.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gwnpxnqub.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gruegnary.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/ghpbkmusc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gclcaoznh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.yfazqb.com/Article/details/gknegktfn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/gmxekpnuc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gbbpxtlpd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gwpyzqghc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.yfazqb.com/Article/details/gydwzffjr.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gnrzbcuor.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gkkmjqmbv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gsjcetuxf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/ggwraircu.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gpenhcjwo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gfvpiazlz.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gyhyyrekl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/glywfqliz.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/genrglgav.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/glpuhqmgi.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/gvhvbwyla.sHtML

[P07] 防抖与节流
来源：http://www.share.tarul.cn/Article/details/gpyeziiim.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gnvachmxi.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gtirckfmc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gqhisqhrp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gkvzescyj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/glolaisbx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/gpabfspna.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gusixlpoh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gpgypibju.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.sjlbkw.cn/Article/details/gxfjdxpor.sHtML


<!-- 参考信息 -->