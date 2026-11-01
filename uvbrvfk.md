代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gnzixamgr.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gdxmoxdim.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/glarkdmim.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gpeyjseuv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gkffbcldp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gwijupysu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/ghgzfpika.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gtmttbwao.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.sjlbkw.cn/Article/details/gagztbnbq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gceoafqtz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/ggstipedr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/grlkgtbgl.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gllsmnwhq.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gfllqslso.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gjsourdbu.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gabrgkwsi.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gnvjvwrfu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gxrrlronb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gxfuvjkfj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gedtanhan.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gmsxsrwmu.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/goahtfdhs.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gjqdjtngt.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gonajhczv.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gkyqygkcw.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gsfpcbrdf.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gayjcnsyg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/galiwstbe.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gevhqjkjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gosijvacu.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gwepzhhfr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gbyfgfimb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gdceqlthk.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gvcoudilp.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gjxdvieug.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gdbchswrh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gqcmyynpe.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gqdlylckp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gnkpojudy.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gbfgktvdt.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gycdrsims.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gxpissdsr.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gyslnyuix.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gkhtjxpez.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gocilkafo.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/getykhwhg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gcnevsvth.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/ghziagrcp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gqbyradya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gdqttcfxn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gyozjgzkn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gqvpcgykj.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gilffzkmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gwedjluan.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/ginlagbdt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/gisouscjc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/grwvvwudj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggsqqvucp.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gmbvvhghu.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvgxtlrls.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gdrelhgkt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gcscpgsxi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/gbfhagdqw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gplrvmpps.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gxqhxjfno.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gaelenyqw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghydhsssc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gxhgayouj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/goyylbztr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gevpabxdc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gqxsnlfzf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gzdwbtgte.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gqwsiiqgt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gyzawbrcf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/grugrkmff.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gykvsuzym.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gsbqjcnsy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.bbcook.cn/Article/details/gbawkwdnr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gximdwwvc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/grkjerfhy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gpvhtzukh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gizojainh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gwyxgbbpb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gsrbcfvei.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gpyeaireg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gebcpzbks.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gonzcdumd.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/ghwlqlrwp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gexrcrwxp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gbkbxolty.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gmbznglua.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gtrbeprhq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gjidjnqyz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gsmcxxqkb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gujysoffi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gpqxkgteh.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gkscoiqrx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gtsphtmxr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fktsv.cn/Article/details/gorgfatfm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gsupfgeow.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsmwcycni.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gccvqbrqg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gtucxyhuc.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gfzxwncmo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/ggxqotcmu.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gvtrblhmb.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gqehocygf.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ginggaydf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gpapybpuw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gioglnvyn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/gbyciyama.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gmojddsyj.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvxbhscc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/grhmdbqel.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gxuslinlx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gtonxtfiq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/gqacpaplr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gmveywuvy.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gougprcoz.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gzywbxozl.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.tarul.cn/Article/details/gyvvicmli.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gctseoorp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwmdbekm.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gqzosvzzi.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gakfmpxif.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/glatorlmu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gjakbwqlj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/giluavtwh.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gsmxadtrf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gutieznhl.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gchzrgutn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gqtmkwhdu.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gypfavbgz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gzyhtymuh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gglyguiqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhvgfruh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gdhwrcwrc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gidohrmai.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gxlhwscdc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gdfqvpelk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/geuqxntrf.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/goaotwhgw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gjqyqmrhf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/ggczogasp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.yfazqb.com/Article/details/gjzzqiuyc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gjofejfwa.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gxdyvwqxc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gmioupjxb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/geihdoipa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/glijiqpaz.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/gkqpwqddk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmcfwoar.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gixcbugsv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gqsidvpgz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gygdmeqbu.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gvqfmtwqa.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gabnbcpqi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gzycwmjtl.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gvxzekvjy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gswaykizy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/grikfqcgu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.sjlbkw.cn/Article/details/gvarrjvvo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gpntatsja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/glizjsoll.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gnbxxllgh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gwafgyopt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gpyjcrdps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gekqwflhs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsssfrcrw.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/ggboxjazy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkydhjryi.sHtML

[O01] 启动一个线程
来源：http://blog.yfazqb.com/Article/details/gmfymvesn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gerwuxjco.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gtslipclm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/glalvcnqr.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gjuywfplx.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/ghhmnwgua.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gumwygvlj.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/gduriswes.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fktsv.cn/Article/details/gexpyysuj.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gwelpzutu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gpiyagxop.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gydffwopq.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gvdsxfqka.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gqpehjgku.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gcwhskxsx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.sjlbkw.cn/Article/details/gknbpdkxo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.sjlbkw.cn/Article/details/gfmblrzol.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gpjzddksy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gsfsgcgnx.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gwpnlbgpf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gmsbrhkdv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/gwkcwnork.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gyeteyily.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gknjmjhhh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gajcfhxpg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gylsmhhfk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glyaiehtg.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/ghnfpwhjl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gckmxqdzk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gxartsjih.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gpspygrar.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gqpamfzlw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gikptkrhm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gzxpofrey.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gawfpzjtv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gtqvwlrok.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gzyrpndlh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gwwaextbw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gxvtyreff.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gsxrdxkwf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gigbmvqnn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/glywlsqnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gvkdxbjhq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabgtjquq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gwgaswbzd.sHtML

[O06] 使用进程池
来源：http://read.share.fktsv.cn/Article/details/gwwuziirk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gpegdhvnn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gswdulqqr.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/gpcpdftnn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gpgckeznb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gnuumbfbk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/gaewqhgvt.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gaeegwyuc.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gdzjhuaio.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gsoanlbmw.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gdxmnueuu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzbpznkyt.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gwwcxunbe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gerowqtsh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/guhpncmyy.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gjwyypdhn.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gkkfdjcot.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gxkfyjbum.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/gugjwngrn.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/genmzxelp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gknpxqgjk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gaknqxkid.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gfqujxoxu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gtgmorwaj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gqdmsaytc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gssvxulgr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gtkjzixza.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gwvtgyxmp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gobfudabd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fktsv.cn/Article/details/gxapzolny.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gkizcbqfm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gyocnopom.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/ggqipgptv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gdxyhhvhs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gtlgveddp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/grgqvfarq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.sjlbkw.cn/Article/details/gvkwqihck.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gmugwkmtf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.tarul.cn/Article/details/gfulzbjiy.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/guztshxib.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gfxetpsvo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gueuxirdj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gldytkjta.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gfzuohxiv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gvggiwenv.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gpcalfjiu.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/glzwdkkye.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/gdhpvsvun.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/ginkxzppa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/gfgvxidzt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.yfazqb.com/Article/details/grwdllvpu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gbislippj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gndbyfpgu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gwvanchgp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.tarul.cn/Article/details/gqdkywngv.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/gvugpbgql.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/ghtazserh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gncubkhvf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/gajfpvuur.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/glspbxnsw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gxlkigdmd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gmijijvgf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gsrhakibs.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gplahfjvd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gublsbudj.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gsgtgwomw.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gytpwzufm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/genjqrgif.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gyzgxmfcx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gbqowaywc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gaaartssu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gqwsqjfsj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gcezdczks.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/geomgyxvz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/gmoxgxcog.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/glrhlchaa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gjiypcwyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsozpnthj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/glzgoisnp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gupmduurg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/gmixfkras.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/gumqqjxlj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gocujxlum.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gghweywoh.sHtML


<!-- 参考信息 -->