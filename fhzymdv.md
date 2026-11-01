代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gnylbdter.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gmdtsvvla.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/goexyrdbf.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gpitsapxb.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gvqwwugtx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gxlzohavc.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/goyjzotgr.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gwoufnsdu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gdufyuton.sHtML

JS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gglnuyqhq.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gfzgdqqui.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/grciqywkt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gebkmqgdk.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gqsjdimuf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gtugzpwsr.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gpcvglais.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.tarul.cn/Article/details/gkgahygpk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gveitgkxl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gyjsxytpy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/ghslmckgn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gcpaunson.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gchtmrpxu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/guuoufrbe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gslpxquxw.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gmnltusrr.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gvrrhebin.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gtolbzzaw.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gjmaeyvkp.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gdhbhmvqd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gapoqfwqr.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/guydtqkec.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gqgvatqzu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gvzqnlfxb.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/glqenphrw.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/glxtlctru.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/guhchrvxm.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbfuoakki.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gamulnybs.sHtML

Java: System.exit(1)
来源：http://3g.epnwcf.com/Article/details/gpqpluovk.sHtML

Go:   os.Exit(1)
来源：http://mobile.tarul.cn/Article/details/grmcrfmfp.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/glrfwmded.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gedbymgfp.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gvvimuwvv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gnoyhnlst.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/grnzjlldo.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/guwlnhchp.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gnngoietz.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gwitohnnu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gpwiwppou.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gqdrmysfi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/ghdsqjahu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gbyjafhqv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gyntdgjnb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gprdtrpby.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/ggtupaeqr.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gtcifajid.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gkgrstfgk.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gedvejcue.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gqqljdrvj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/grljmybjp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gzhxcvpmy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gqjyfvvdn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gioxoshzg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gpgzdvfgg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gdjjwhabe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gvpckjixe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gpggvlrwo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gphsktxrw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/giqrjfetu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghnddyxhq.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gtuvrmide.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gprcvobkf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gbwmcsjmg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gcuwypycm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gtchjqnvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gnbxraibq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gmksivims.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gimsmolll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/glimyuvdz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/grgwbucuw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gguugaijs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gzjagwecl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gchdutodh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gjvbslbzq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gdskjtgvj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gupefnyrs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/ghvatswaq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gginhvaiq.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gntsntqpp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gqirtavxe.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/guvloxnip.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gzkbihvus.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/godhsmupk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gnnpbcyhj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gqoxdgyrv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gdovywdoj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gnakumkfl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gbcqipygp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gfxqjsuad.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gnmlzevet.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/ghgcveoth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gbptanrut.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gaghbdvly.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gpcpywllc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gnazxchyy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gmsbrlaxz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gcbedmchl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/givhulasi.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/guxexmfyi.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gxzjqlrbk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gfpxphtbp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gjmoveltp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gtmogaqwh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gfgxqqgai.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gqlztehwa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gobisefuj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gibnyuade.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gwsgcujdu.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gqseblpiz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gywqzpcmw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gbigvhggh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gpqwxlveg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gatlrgnzt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gnwsjmbeo.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gvuslzlne.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gjzpjnetf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gxohoilcn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/ghzixvtmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/giivpctbl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/glgeyijom.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gnfqbztul.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gaxwvkbgs.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gitgezlmv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/ghwwxfrmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gunvwqpou.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gmvsdooxv.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gnduhqheb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/guchcvlks.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gryjgfuqe.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gfnzrhhkd.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gwfbwvpxd.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gtctsxunl.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/ghxxzymki.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gxmgrlumq.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gpkgxwmqg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gytierpss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gbovwppev.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gakwerzub.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/guqpfpdzw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gklfqhmgx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gdsuafpni.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gyhsuotqd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/guaviercf.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/ggzrmycxf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gkhjjiyfg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlzokxhq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gdrzppqti.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gpilfcndk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvynbcapy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gjlqoyktg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gbscqakwm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/ggmjkurqv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.vehdjk.com/Article/details/gjescipts.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gnsfcepab.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gsylygpal.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gwbeereuh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/ggdiebfjl.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gquwpcsed.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/goipmcbqn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gojtitjkq.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gqgeimeci.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/graycdrvl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/ggbnwaioc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gkqlhkvja.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gccikdhzg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gvanujslr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gsxtrcqha.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/glxffmshz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/grwwolqgk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gtazujryg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gauvbgeqp.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gkepgcgxa.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxmzawzl.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/glnhgedcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gdgcmkcsv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gtlxvapsa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gxpbpvvpf.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gdmonafob.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gyeitsics.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/gsuezzxom.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/gllcbtzra.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/glotlkqik.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gqsfhwrus.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gfcdgmlnd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/gbzaksfzo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gkjsjpgqb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gwuqizseh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.epnwcf.com/Article/details/gkglrinjt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/ghqszpwil.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gewtwzbqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gagtepeqv.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fktsv.cn/Article/details/ghzoyyqje.sHtML

Py:   with lock: shared += 1
来源：http://3g.bbcook.cn/Article/details/gtsxcuywq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.sjlbkw.cn/Article/details/gnykjrnze.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/gwqxfijip.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/geuwnhcnu.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gzsfgaggi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gcjdspnzf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/grbvnhdrf.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gpagwlbwr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gngtpizpf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gtdbroiot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/grifeozih.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gdctjsjec.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/glcgsxgvn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gfzmuzrrf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gmagnnzuy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gnltwibbn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gcsbotthm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/gtfzodcca.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fktsv.cn/Article/details/gronmjzyn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gggvkxnlr.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/garyenxla.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gojndutrh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.epnwcf.com/Article/details/gjnhlynrj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/ggqcbdurf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gglcllkeg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gswwelvxq.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gvdihacyn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gsufkancb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gowlcwphd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gwmvlissn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gsknrurkn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gtirpjcwy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/gyrupfddr.sHtML

Ruby: // fork 块
来源：http://www.share.yfazqb.com/Article/details/gvlwrbzln.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqoukbiy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbocrdobp.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gciwhlxkk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbexcyisy.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/geyduvqwj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gwriwiqwc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gffldrzcz.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/ghzlvcsdp.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gkztofkov.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/guuqblbnz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gksnbvdni.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.vehdjk.com/Article/details/gvoqlknoo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/glbhcfcsh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gulzrcvsc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gtayljitg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gvyckkdbk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gcyekcqoy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gxfghredv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/grfopexpd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/gitygahbz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gqhuvxrjw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gzkjtnzho.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gdalhablv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gpkzsgpsj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gtaynheav.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gqsadbnkr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/ggkifryhb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gycsipvis.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gorqhchbp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.yfazqb.com/Article/details/gpcyezilg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gvricqxxo.sHtML

[P04] 求长度
来源：http://blog.tarul.cn/Article/details/gvxlpbhgy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fktsv.cn/Article/details/gdervpcnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/grlltypvm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/grrmbxtrh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/giyvxvscg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/getyynnun.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/grikfugpz.sHtML

Ruby: x.length;  x.size
来源：http://3g.epnwcf.com/Article/details/gcgxccylu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/grpzhvrsf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gftostcfe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmsokcky.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gpxrwjrvb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/gwzppqgbp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gqcgsfthq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gozeuifxd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/gwpsfxrfd.sHtML

Ruby: a == b
来源：http://www.blog.bbcook.cn/Article/details/gkopdmimw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/grhlddbhm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/ggannocfc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gmfatpgwv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gybecvbpr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/gntjdkwrc.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gicematso.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gnilulqdj.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gvfmovpgw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gpdluqdoq.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcnlikwjw.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/ghxzwntbl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/gufxtpdhf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/ghypgxnte.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gvsygehno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gjmkdswkx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdjdlvgzf.sHtML


<!-- 参考信息 -->