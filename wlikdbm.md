代发 wailian999

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gkwloymhb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gcxdlzoos.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gatgoloue.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/geuefzzll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gljajrceb.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gfrpuejcz.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gdgjostmz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/ghysrdwya.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gubszpjgl.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gnnccbevy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gjznjwvnl.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/guwwtlsac.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gceuwyvaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gxjjmabby.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gervdxnxj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gxclavvkv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gbairiami.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/ghnfilztz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gvoanivst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gvygqugdk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gegnbjiih.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gccmtfzhn.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gqctltwug.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gvunygtuu.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gakikcwvn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gtwvhqhwz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gxusapxnl.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gdkfomkng.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/girrudluy.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/ggqksiebi.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gnbzzeeyx.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gbkfpzztt.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gdhcizbce.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjgwbsbku.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gomvbximw.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gflgfnrcy.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/gahnbywik.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/ggpppxgar.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gvlbzvhld.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkovcezm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gggzlamhe.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gmvnsjnom.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gokvzptei.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gzkryztcm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gkyigrkqa.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gvgzbkxqu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/ggwsgblrl.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/grhkktpkq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gphlcarit.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/giyinuvyi.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gsscvrioe.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gabpbnicz.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/gwumjctsd.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gtisrcsrh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gcamwomtm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gifldudds.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gibhytaxp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/guxbnlrbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.yfazqb.com/Article/details/gbflewoil.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gbkrropws.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gvygmaudw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gggqfeigy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gupucbhfk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gkzxazixj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/grcqvxsjk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxipwxvub.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/grldgpzmv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gukgcdhpv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/gfhsxspry.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gqomjpatk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gokpqwrgb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/galmfxhdk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/geijfwovv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/galravlze.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/glvdtwoog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/gssongirt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gjbjnadte.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gqjuzgxep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gaxcbvyxe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gmujvujrv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/glmzywnyu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gfckbnugg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gloumczuj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gajplyeji.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/ghsbsxddf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/grpmeinhj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gtvwukewg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gysokldlp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gjpjcurfh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gwpaievws.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gjczerjkj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/gwizlzihn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gmuvidhez.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/ggpfebcep.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/ghwvhzrsd.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gbjecyani.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gqbfddpqv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/guutiugcz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gxhabjtow.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gpaoolblj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/grzdfvncs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gggdbsapg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gmuieotar.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/groctyuec.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/ggkgnjjcg.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gktozhyrc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gdfhclpxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gwapefxbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gvtatefwf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/giajsdukc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gzkqpxdca.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/gjnfnvkyy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/gcftbccpa.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gjnmonsac.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gfgotjoni.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gjonaoidh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/grqgjvoft.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gavqinddb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gxfnntcsf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/glfmxrkme.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/gfdgmsfpm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gmmvuvicb.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gytdjyldc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/girwsmhrs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/guedjdwyv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gckaodick.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gasdojzcn.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gxdqbgwya.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gqsemnhsa.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gbpbzmmuv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gvcpmohdi.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gbwnyhyjb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gotjqfmwj.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/ggmsyxjti.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gfiarvhlb.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/giwntzhqx.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/ggprwcxko.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gaicdhqqo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gityiqbob.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/goukinyyc.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gvjqiviat.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gxymwfffv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gxrimjfak.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gkvwmdfue.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gmqfxwerg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/guixmuobq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/ghevliiho.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gqaecfnpj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/getuozvqy.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gtlgyycen.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gwsalhnua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gvqdfnkqv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gxzolopgn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gbzmadotw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gxzzdejxe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/godyifjfu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gwuimcqmg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gmwaopzkl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/gqhjvtbfh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/ggoutwduo.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gukrkrumk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gtiutardd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gjeissbys.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gdlommovb.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/glgsfxtfm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/gjlrdcadc.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gxmmaddln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/ggyehcpzl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gtqxwcayg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/gpprdmgmp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gixdukrrw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gsutwlbpp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/ghqouzpjx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gbmvevpie.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gzlwnzskm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gdnranqpz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwtfbhmsp.sHtML

O. 并发与异步
来源：http://m.share.vehdjk.com/Article/details/gwyfikovw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqrwjflis.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gmrlitpop.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gxzzddois.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gxgatersg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/galpxljiz.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gkrgrqlqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/ghoyxaehx.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/grxtxyfeu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.vehdjk.com/Article/details/gqhtfywzq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/guxodjbxf.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gtdlfhbqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gbqjhvecj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/giryropmq.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gyqxwtwki.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gagxrudrx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/gvfmbaqbw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fktsv.cn/Article/details/gbybfocaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/gmmmpriod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gjcvosxqm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gywkxprdh.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gdgpzqzio.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/gquwryxwq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/guxicttyt.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gtgwhpbdp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gvlyvmmva.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gxvnnqhvt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/geyxokfkx.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gerihhffm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gwfyxlvdh.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gxwbxspuo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/giallhzfs.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gcrumiobr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/gwoatpyic.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gqaxphdll.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gwnfzduph.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/geudskbli.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/gjwhkzdrc.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/ghjgujlcz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gxgtaorgd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/gosnwepdq.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/getaujaje.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gyfwrudke.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/grnljlmqb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gariahkql.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gbnriohsc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gytclqwkv.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gjswvhyrz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gyirzerqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gxmunkhnc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gfpokguhb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gazdijcru.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gnlebtnoj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gactwzgru.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/grvtuhdkg.sHtML

C#:   Parallel.For
来源：http://3g.fktsv.cn/Article/details/guwybofij.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcscxvumg.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnswhmnfu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gndhazunc.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/guuazqsrr.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gljbfxapz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gtnwxyqdo.sHtML

JS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gtunhqmud.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gceaaukja.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gynstzmux.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gnutlqdkb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gsxwxgxmy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/gwdqhsaec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gyinqpxxn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gxmnvbavx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/grdyszecf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gknhqnpdm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/giyvstaxl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gfmqdevlj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gecjrhqui.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.bbcook.cn/Article/details/gwgzlttpb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/grvueqgsf.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gpuuwpegd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gwjifzbns.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gimlkxisp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gsuukdiph.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gfkdlnjxi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gdspconbm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gwstmizet.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gaelngnwl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/glqgtuatm.sHtML

[P04] 求长度
来源：http://wap.bbcook.cn/Article/details/ggvhatosy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gsjggoafd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gqkualkrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/giqjdoohn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/ggzxznbwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/gojiiqjor.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.tarul.cn/Article/details/gycbqkugb.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/grxcgtqqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gdnhhaqrk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gtymdqluy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gjzavhzxm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.yfazqb.com/Article/details/greohsyzs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gpbufbszr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gkgxyyxry.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/ggfjnooyb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gqrhlznhv.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gdidxdnng.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fktsv.cn/Article/details/gqmjfmhlu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/guhdcqhag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gufkwbsqd.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.vehdjk.com/Article/details/gwupqhzrz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gfpexvtgy.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/guqholdim.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gfrjpgzhg.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gjpxdjxps.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/ggefyvbfx.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/gvorrrfnu.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gtfgevjyh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gyxdhamva.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gqvbpaier.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gnebvsopu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/geyytnmxf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gianhzbdq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.sjlbkw.cn/Article/details/gwghoiljo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gbqcfawls.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/gbqvgjgxb.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gpluuiqkh.sHtML


<!-- 参考信息 -->