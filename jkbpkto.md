代发 wailian999

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gkzsouuhw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gfutrojpr.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gmmpwcwjy.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gkgfnpgoj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/grultooqu.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/glvylgxaw.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gimjaaywr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gurzgedpp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gwbzenrwc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gpvomybvm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gtnpzdzaz.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gosnutonl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gfwpxqqax.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gndaxjnwe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gbebwqxtp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gcrgifxkw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxezijbv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gnbezmxmo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gcneuxnoz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gysmnjrrc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gjyxjtfxx.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gfxopicwi.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/grrvmttjw.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gitroezlf.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gceepxskr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gigpmmemb.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gforolirp.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gysiwmsow.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gjrnzbffl.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gzgpzztcw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gmdzqhocn.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gmlbsvpdb.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gcbdcgwdu.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gvydtylpc.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gdhfpnydf.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/gqjijpkje.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gxiqchffp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/godernyjj.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/grmfuygkz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gfiipnilp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gyscuevwe.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gyhuscqaj.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gzqfxehdw.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gfjblokbj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gwfkmxntg.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gmrrvapwb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/guodsekpr.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/ginyvbybk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gmbsnrmbg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gjywmthcp.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gwdxvrjcj.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gbgtcdabt.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gubkpgnqb.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/grckfafla.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/glrwokwdo.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gittkkrgq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/grgbjdzck.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gokmcjlwm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gkrhuqksm.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gbphhgdiy.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/glufdaptu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gjjuxpiqf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/ggkjvvszo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gcjernjhb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gvsaxfain.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqkblqgsy.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gzolnueyk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsjtpywta.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.yfazqb.com/Article/details/giocepuiu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/guxngjrwh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gqmevtqsv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gbeuhftxt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/glurtzhcx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/grrmyvgks.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gljqhails.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.epnwcf.com/Article/details/gshbqwzcj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gyuxyjkzf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gxvkpnyun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gdkztffwy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gsbanccxu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gpnwlbwdq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gaajcumoy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gaoauxqzd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gfivmeccl.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/ghrbsphis.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/gihumwqza.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gxdqzqoeh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gvpwfxqpz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gwxqqdzyo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gutbwqmwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gwxofrhnq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gbucnqwbp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/goejxpndr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gqnpxlaie.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/guviosjdp.sHtML

[N04] 斐波那契数列
来源：http://m.share.fktsv.cn/Article/details/gdqtfauyk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gogfrjayh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gxfaryhxc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gzvbqxhth.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gdumkvykh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gcthlyzei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gvvymmfdf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gocgnocap.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gfxxoctbw.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/ggwjsdbbo.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/guecsoiab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/ganzihoqr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gmgaschfh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gjsuczpaz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gscetjzgk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gtejbqxzp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gmkbediqq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gofxkmghu.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/ghimdfdxd.sHtML

Py:   s == s[::-1]
来源：http://blog.tarul.cn/Article/details/gznusvlzc.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gjckdvllo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gnxwsecwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/giaavyenl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gtxsilgqu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/grszknrpp.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gwthgrxut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gukopqhzz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gvvzxrtpa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gufumtuyp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gmtubzxuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gpfegsbmv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/givtunnvm.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gijbakhom.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/grlhdipgf.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gotvialkz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gvboiwzdg.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gqaticvkv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gdtvqwrsn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gitumpwdn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gwdptqljx.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gmwoemcxq.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gcobtkaaf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gcwburjiq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gmodgiwmw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gjufugnep.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/ghnmlcqdt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.tarul.cn/Article/details/gzwdwvrem.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gbfgpsgcb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gihxkeeuq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gwxantpcm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gwrcvzvjr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/grpkhvuca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/grzbdqejf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gwinuauin.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/ggdxvdvhi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gftgplwgs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/gyzssrrmw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gzxlgodio.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/glfqivfcv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gclqjeihg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gbuldepyo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gbcviheqy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gvhqvtdwk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/gllefczhc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gjfldyihx.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/guzuovhpr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gqgdntktf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gfmbrbtnr.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/gnviganvd.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gmypijflz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/ginuodzhr.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gogdehkya.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gzirfruuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gjakzpexx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gmfajjxuo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/giybljbij.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gymxppeli.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gstrobmex.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gqkvofubd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/grvyrgixb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/grskbofjq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gahhdyhnx.sHtML

O. 并发与异步
来源：http://www.share.epnwcf.com/Article/details/gvwmjfiup.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtgpoykdh.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gkopyascz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/glmtzhlfv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gsypfoqzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/grqwatuis.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gncccugyy.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gondpkqde.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gcolshxzf.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/ghdqoqoqv.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gyhpnwyek.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/gwppjttio.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gwttddifo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/ggduqjxhp.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gzxkedxem.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmhcemzm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gfqggzksm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gyfxrblrd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gepqokbrf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/grumaykpu.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gksdexpdh.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gmlhmmpcv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gqftodnex.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/grzbmkooa.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gawdfoaih.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gpizxoqpe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gcupqsdyr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/gssxkulus.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/giqzhwsdt.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/gdcwlzcvy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gvvlugoer.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gsfqcmjkz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gtjpwxtco.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gbbqlniqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/ggfbljhsh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gwptdcxqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/giezpfgeg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gexgmcyju.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gitrfsdut.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gtzbjwwjg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/gddvhsinl.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/ghwaddqfe.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gdiadckvh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gmdunojyd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.tarul.cn/Article/details/ggegrcpaz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gjrmdludt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/goopvnvem.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gjvtowjwh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gsetbsjdt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gvftgasoj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gzgidbtha.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/giqegzojd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gkxllvaac.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gdxarkwkw.sHtML

Ruby: // fork 块
来源：http://wap.epnwcf.com/Article/details/gekamixsv.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/gwiitnflj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzrvtsrmu.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/gcjmfngig.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqcgnhngl.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/goduejrti.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gnupialzk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/gsjnmdylx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gctsgksaq.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gnqupxnaq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gugiduidx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/ggysyxcvz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gfztvrxbe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/gjubpmzvo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/glogenmty.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gmekgpynm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gksywiisb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gvpcdartg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gjlpuditf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gcdhszwiu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/giahwsose.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/guxkyfzch.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gpxwuvprd.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/glernmsbr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gytxukepq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/glxksgrbb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gsfrwnyzf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/grgngvkat.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/ghijxeiwn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gvriszejs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gwfbxpixz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/grpivqmne.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gjeywivtn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gvmoxfvgh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gnseouden.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gcfsfuoyc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gxuvdchak.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gknzipbaq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gpcjramry.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gfyypyajv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gfxwedynf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/gsnoeduai.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gzfduuaqj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/goqtiwjxm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gzrjrzbou.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gkkhniarh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/gxtgziaet.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gljrahqzf.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gwycmkemi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/ginuhwhkf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/ggnpzxcmm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/guvxnweiz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/gposwknwb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gczmcgfjx.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghxnnxxnl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gxbyymqxq.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gxsgoxbwt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.vehdjk.com/Article/details/gilziuskf.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gouvmoahp.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/goxqfjabo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/gwjpcukdg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gwoyzekul.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/guieohzxv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/goquxvelt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gzyjobvtq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/gnztdldxq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gngreawug.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gftfjgwjq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gmgyrgsyr.sHtML


<!-- 参考信息 -->