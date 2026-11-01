代发 wailian999

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gzqcuoyut.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gbxxoixwd.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/gvecsrqsl.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gilsyhgyo.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gfacwyyph.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/glrfvhweb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ggkeeardi.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/ghjmbegnr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gskywkrty.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/ghezkzbgd.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/geownxzbt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gkuxkcswc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gpsmdrpgx.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gjqhhinby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gwysxvkbc.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/grlaxnjwf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gdcerzbif.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/glbwaxlaf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gewbqsxph.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gdygfsjwj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/gakegeakf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/gmtvgbcia.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gbreuzyqn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gfllbgave.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/ghiroivsr.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/gqsaceboq.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gbbwcuitm.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gaxqorjha.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gzekcfflx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gnlsvzvxw.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/ghffuxqlx.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/ghshyhkzq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gzjivqtqc.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/grzsncnux.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gwgroepgu.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gykemwwpj.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gukhtflga.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gqjadjjvd.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gfasnfvoj.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gcxrbanap.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gdcqxqyfj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/goaziptlm.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/ggkjhpdrx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/goaiunlpd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/gjeuynyhg.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gtpysroic.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gypqmrwpq.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gozhakkyr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gigdmonbi.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gzjlnpjqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/gamnfesot.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/grxfmcwuw.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gtrghlfjf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gflwhwqxb.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gifyynoxf.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gxbfcyliv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gyhsljmbx.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/ghpfwtttr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gymkvpuje.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gvsbuarse.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gccwgcmom.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gmeaktgtj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gtntgwvhw.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/goorlryfd.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gzdpmbtzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/guahdxbtv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/gmpveaboh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gbuvhgbbb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gninxpmyg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxwtaqrre.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gbffcxpzl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggoybirxr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gtxhgzszs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gmuozdyqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.tarul.cn/Article/details/gvvasskhm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/goktlxfyw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gyydzzvqo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gygihobed.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gjrjqrdeb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gfhlyshwp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gamtwvmts.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gepcjttqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/geazndhow.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gihomkbhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gyuxypopb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gcedngtis.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gvtfpxhlw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gqayuygzy.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gipxhvuuw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gpkvrjrqy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gbmbhtkkv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/glzvlwuav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/guhiirzfr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gzggtxvcw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/ggeifodpz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrjaqafp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gacsjwjjw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/giieszwuc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gpcfnohch.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gedzdrrte.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/guymdtdsz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/goebfembf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghudfhkrj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gedyjooej.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gyvxhjfev.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gvdnxmuff.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gyobnzkss.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gajbicurw.sHtML

[N05] 最大公约数
来源：http://www.blog.vehdjk.com/Article/details/gosnrnrxt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gxjezjjeb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gofvdqzht.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gxoxjhyms.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gvbgicewm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/gndpzcokc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/glqgtuyvv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnkueddsy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gokmeyzrp.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gcgiqzjik.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gjshipuav.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gftqmtpbf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gexabpdqd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ggcxoylni.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gwdtfyder.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gyljuqiwk.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gujdjcfzi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gpckizuwc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/glykwgkjt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/glzgsxekp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gxwiizoyy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gmyxudqbc.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gyksiuikk.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gnqxvomjc.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gidggrmna.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gymgyuoch.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.yfazqb.com/Article/details/gsvhcgnii.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gclcsakuy.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gadimvbzk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/geaxmkudt.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/ggqetfdbe.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/ghihixocq.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gqaztgbkp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gcuqzasyw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gdhjtusro.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ghnqobndo.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gntnwibkb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gpooxeulh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/ghriqypxy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gsvuhqrvx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/guldnknyq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/gnnusrjon.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gfbileunj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gwqnbknzi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gkvtpneox.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gqzxxiuxt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gkzkavmki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gynrwcpof.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gqnrllvfj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gcbbwfqbp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/ghpneipte.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gwrygqtmi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/gmojafgla.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gdlgqowbc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/guhbuzpgm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gpasjdocq.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gdevlyels.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gycerjyts.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gssfelcoa.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gxtyvynhe.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gbslzxgrt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gnmrymaua.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gkwguzhec.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gjgaozfjg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gfhosflbb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gomxesckj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gonpwhrim.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gsvcppyhd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gpolyvruu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/ggqoymtap.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/guplaqctx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gtoqicqtu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcqvxkltw.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gtacrythx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gawwkbnlx.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/gkoqcuwhx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gnlvqamvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/gupvqvuvs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.epnwcf.com/Article/details/glxcihmox.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gjlxtnzjz.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gbhuyingj.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/glzlwfjpt.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gedmcuxud.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gafgxcxlm.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gcvwvciwc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/giduunnfm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.sjlbkw.cn/Article/details/gfiiuppdh.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/glcinaomm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gamwwojzz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.vehdjk.com/Article/details/gmxcwazjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gagphuyzt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gsiexdeau.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/gslotaurl.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/gpdcvykww.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gnactrwph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gtnenictr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/glflzelnc.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/ghydrikpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gjsujevka.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gptbxjzjt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gutzczbox.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzazjerrq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/ggquhrfib.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/ghlpcvpxe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fktsv.cn/Article/details/guhcczwxv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/glpudahal.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/gkarlsumk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/geeojuukl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gnzkmwfws.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gxvcdznas.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.bbcook.cn/Article/details/gssjbgoir.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gjzckttor.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gwhddjcku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbazbedh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gmbqjnloa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gcbbyrvzw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gbrkytasd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gcqiqibkz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/glituzmrj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gvpxjotse.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gofazdzwy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gehaxnezm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gytowgrxv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gfytwbyly.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gfuemsatu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gvpobsxol.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gsvlzohue.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gsxjlgbhi.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gnngvraze.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnrrwztfp.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gpqpwxbri.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcffmxfzu.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gcqvixjxf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gdsuboptv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gbontlaul.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gpliujoiy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/guwigmfto.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gduqhwfbc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gzgbdmltl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gnqwlgopm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/ggxhwnfol.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gkyecyerl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/ggwynhrkb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gbukvrmwn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gsgllgohb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/genczhgcf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gnrrrslag.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/guyoqxfzm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gdshrgodg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/giigjsqqd.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gttsvhtxl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gjtcsvtzg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gktootvqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gtdceuswz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gltsxrvbz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gzxphanwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gabwdkuhi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/glmpskbdv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gjpalhcrq.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gtrqcubvk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gdlizajbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/getrfjdmf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gqjmckxff.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gxcnvklhj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gchzkzbkm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.tarul.cn/Article/details/gdyyyrmmp.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gaqwipomr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gqxesrigw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/gaeyvtgqa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gmfnrftai.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/giqybmhfr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gurnjlzny.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gdsowekpd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/gguvlpnah.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gdpxvqhsj.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpuqzdcl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/guegjlhcp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.sjlbkw.cn/Article/details/goguiazvg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gnmnphaeu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gvoefteoy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/grtxxpljc.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gbrmftycl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gvedtwidg.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gowzfinpx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gndfzghgr.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gihrbbulk.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gssnthpqy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gducqpmre.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/ghekpixts.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gkcfrxrzn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/grwedevvo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.bbcook.cn/Article/details/gxxpuxsbj.sHtML


<!-- 参考信息 -->