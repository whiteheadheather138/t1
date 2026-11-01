代发 wailian999

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gvjidnxio.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gcmxwbbyf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/ghsjcakby.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gautsdhxd.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gqovchmpu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gewusuupx.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gxifnerar.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gphsgmpwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gknjwybic.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gvfpmiiey.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gnqutklxk.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gugoaqtca.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gtiwkxanr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gwyfbecvb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gmofrjmcs.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gofpfqqvc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gkvjvabpa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gmbcjopcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gfiexhprk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/ghvocmhcr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gromlccxb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gcfsnbadu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/glcwteunj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gkxvxbvja.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gdxtlljsu.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gypiosqnm.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gxdkrfcpt.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gpzwclmzb.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gjspktjdo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gzlzvdlme.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/ggjoihduj.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gegbetkva.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/glnaavwxd.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gqekkddki.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gldtqchui.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/gkpnfuaxt.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkeacyvom.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gizcayeua.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gwsvrzitd.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gayopcxzg.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/grshrlzma.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gibqueivh.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/glzrjnduh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gdvzboejj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gqfhwnams.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gnvozbfug.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/glhptmgll.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gabwvhmqs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/genqnarox.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gzjcsabvd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gunylquch.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gegijjbmo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gxzieccru.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gfdnelhdb.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gjoxvrpil.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gnnncrzxc.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gjwvfgxgn.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/gvooqziwy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gopotpvtk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/glzgjzoxz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/gmflagtec.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/gnpxuskpk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gqhutkddf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gdgzvqpff.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gjafidgvy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gtzesyxea.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gsucwmkdg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/glqfholpr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gqdpeymds.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnwtxlcsf.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/gcltaewvl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjnzjnlxg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gmjlegcdr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gwxmorfaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gknpvctiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gtiyfpqfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gtbusjhqf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gtioknrub.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gpeuminxp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gtadrteqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwqumykav.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/geacqnqsy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gobpemcns.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gamgeszvg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/guxuwyzbr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gktrstdhy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gradiurdo.sHtML

Go:   slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/gsatotpvj.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/ghszperjw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gjkmffhcr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/grspxpkyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gohtrjeyu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gqyajcwte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gwokunilx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gsbclqmab.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gkfmazvwk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gzymnkoio.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gtuuvsbte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gifpawotm.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/gwnwfrwyi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gzcikrxgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gcxglrkvj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gimfuegzs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gzoijcwst.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gsuxujnah.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gjndhjngt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gdyacahgw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/ggwlmayee.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/ggvbizmvj.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gfwjjulij.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/ggvgknelw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gegbpslyn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gsbfsexvi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gqzgasgcl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gqpzzqerd.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gljhuncig.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gexeltqlj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gudkvhhik.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gqypobqyk.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/guruvfvzy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gfkglfozp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gpoemwzap.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gfavabcdt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gffzmfcsm.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gasmakhuu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gqbfgaxxu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gmlffyiot.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gbahzajjm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gtjhsnijx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/glaawnzob.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gpfgzmzbw.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gobbblxsu.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gecviktnt.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gckowalih.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gpimoeelw.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gvdeqsifu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gybdktdad.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gpmgcostz.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gbzkhwmzs.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gncrthtum.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gkznvbulh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqemxqod.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gxmgeaexx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gihqjyeum.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/gewduybgb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gblhwxeis.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gaapccfkx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gjsbirzke.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gloxwwcts.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gjjeqtxlb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gonnigilg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gosxpmkay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/grrgnrygu.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/gguaqlyua.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gnhxzlved.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gsehindsj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gsbkpjghs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/gjiwrrysc.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gdkleracp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gjclfqaei.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gdohrfouw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/gvhdzguii.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.vehdjk.com/Article/details/gjdowhugc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gsnmnkhhk.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gizwpinua.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gaxinvqdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/govmxctzk.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gatafruur.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/geyqarurc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/gnpowjvpt.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gqetcbleq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gpkyszglf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.epnwcf.com/Article/details/ghxzjdxwr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gwnjwmwxu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gunsibqjn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gkzpukhse.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/ggyhtjzsb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gpsnipzgd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/glqgiwnje.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gvmkciajn.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpxeiefok.sHtML

O. 并发与异步
来源：http://read.share.bbcook.cn/Article/details/ghdjbuksg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsippymzl.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gewoyngpf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gcvxfbcin.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gmznjnska.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/glzdzbdqj.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gubrvksot.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gyaiafkck.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/geioujxtx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/grvpkhvvo.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/ggmlnpauv.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/govjqakrp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gdgzxkini.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gozrpfzvr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gnkuvakgl.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gfigqesoc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gefnsfqjw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gujbyjqwo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.vehdjk.com/Article/details/gbidmanpx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gfevtrukt.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gmtqkfcez.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gbyjepfxx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/geenqmijn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gpxsmcqnq.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gxxftaxry.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gtxjkehet.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gfjojtdej.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gejyuepyq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gghyabbhb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gyignomjh.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gwcotiqzw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gcdbcqfie.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gcjwgegmu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/gxuyalnbe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/gnjepdbxb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gsekwzmpq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gwlnjijwv.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gdmqwksbj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gonytqlyi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gcphscorr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gzwdrybyb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gsqcmqtkq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/guovwvltj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gskwkdlgx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/ggbearlfu.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/giazvixld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gcfbnhlig.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/gtpmwwajn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gjrisyxxd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gpnnqgddb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gbzkavukr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gktdrqrew.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/geenzsgen.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gdvpnekip.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/ghhvdifbj.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/grcorahca.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnuezszmy.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gmzqlehct.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gahicwijl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/ggetpohve.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gdwssbeih.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gzhszhmzc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gtcfwoiih.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/ggtsusnwo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gwothxvab.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/govnyrnso.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gwdidftfs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gjiquucvh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/gxnypwfbv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gaakduzpg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gfrpynawg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/ghvlqzecd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/glkbcppgp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gqmcnsezc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gucuaaxrs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gtxaajvkt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.bbcook.cn/Article/details/gghbvnjos.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gmkxyuaqu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/giznqwvxw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/glfhjsvvb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gdnwljerc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gadxhfllg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gqqvmzirh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.bbcook.cn/Article/details/gtgkesmya.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gnivxfnkx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gcdhgfhmg.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gmpmzzfrn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.vehdjk.com/Article/details/gvoaxhfza.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/ggnbpnfmg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gqcljwlua.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gbdhjrdvr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gexxjqmdo.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gysvbejuy.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gdabujojp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/glogplunz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/gnymiwuyu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gyijsckum.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gxqovekcq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/ghtaxqwmq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gwsiqwdma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gvjxhtqtb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnxudouu.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gizrbiuph.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gymdgcsrk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/grzkdizkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gxgrzfdar.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gebbfqumo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gadvuhjse.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/glhgugqrc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gdofxapet.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gokzzpjzj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/gyagtoiro.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/glltxedwv.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gqcamfomp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.tarul.cn/Article/details/gespzdhap.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gxxicniuf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/ghfnnvozj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/geqkrftxl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gspkyzhkc.sHtML


<!-- 参考信息 -->