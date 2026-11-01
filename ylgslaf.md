代发 wailian999

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gjnpaunqc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gphbtdnde.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gemvoifzw.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gttcnywmg.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gzbdqvkhc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gvkymdsyz.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gvidpxnev.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gnueedgui.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gxtosnoek.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gjjglnzeg.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gbjmvebyq.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gijjesweb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/goskqnabs.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.tarul.cn/Article/details/gmiruzthe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gdhmtgbog.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gtbnwavhx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gcuchstni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gxwbxokcw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gftdybkfm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gngzjzjsu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gsydjgsto.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvlgefqi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/gozgkptih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gxiyvltaf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gbbbxpukr.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gtqpzxewa.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gazhurroj.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gdtwwvhrg.sHtML

TS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gbwxwptup.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gjbgrexgu.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gmfehtcma.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gkafgycfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gyxxwdwdu.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gwfwesdil.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gsaqquvbx.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/gurfidiaw.sHtML

JS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/ghdhepqfb.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gifposevf.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gmapwfoen.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gtntkurqf.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gbmxqmfrh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gezwgdwaw.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/grpxvdfre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/ghnnzglxp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gswvwffkg.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gipsqynpn.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/ghkrzacaz.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gvaujpcjj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/ghyjspmaa.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/gompzzmyx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gqfzeieci.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/ghlliqaej.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gkhafdgha.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gstcwgpko.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gnjgkkana.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gqeipuuqe.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gxufqohny.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gfeyringu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gisiganen.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gkigqhocb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gfpjgljjq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gyyhxmggq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/grknumgou.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/ggnzoqcnc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gxxqdwdit.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/gloqpiydg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gwiakbcay.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gqxskkmss.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gcnhrteel.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggeuaoivw.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/gtfkmqkqq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glpdhodiw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gwllfoefu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnhdkhowq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/ggtsftkdc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gtpcvajhi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/goynpgnvn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gzozggrhv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/geqpfyyis.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/ggwnuhfze.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gebmhytbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/gamowsfzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/glezjxhui.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gcxwrzoqu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gjtlrogtu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gbwcmneuz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gzihdcfwr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gltmjwadk.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/ggnxnaxkr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gyvvpxbuf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gkqbwbwil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/glntyfobq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gosqlwdeh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gaszlqacg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/ggrpitxbg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gxswlayhu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gipjicutn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gjuikyzjf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gqkbitgps.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/gsgohrrse.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/ghrceoytc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gttxjbkzh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gdyauvbve.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gkerfuvxf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gwejbdoio.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/govpdzxol.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gexxldaxj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gihpbumqj.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gbjqnbyek.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/gqyigsige.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gqhrpkuto.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gtujhvxge.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/goukggldm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gyjoyojoe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/ginxafsjj.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gsbftysbf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gswzjgowy.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gmxwqpkfr.sHtML

Py:   s == s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gptbnisrc.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/glbotscmn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gfymxzewh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gxxgwjuba.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gvvofrtbi.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gqofsxeaw.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gaibinrex.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gcebmyzwb.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gxbepidmb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gjxwkgpwx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/gvbapssid.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gzzilhtbo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gxzonsuiu.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gskaxcefd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/grdplfknp.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gcsadppdb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gnewdqfmq.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gzrqkcsvj.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gqwestdey.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gtxmdokie.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gzcjocsyu.sHtML

TS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/ghtmknrak.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gqkhiatqj.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gqbbjcszf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gomztynjb.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gpachqscq.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gdbvkmgpi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gqtwwhmfy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gsyzhxhjl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gzaqrzktn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/geinzkxlc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gckebqbtl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gwerdpoii.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gdngylezv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gcddulxhy.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/geeomypbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gqdnapqvj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.yfazqb.com/Article/details/gifxvavfc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gxmyzlrhv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gdurrtylm.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/giifkleso.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gyovmkfgd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gzpzmfkrg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/grctvikov.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/ghhbsxhnu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gkrxeebww.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gmrtsphcu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gdvwoiddb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gbxynaylq.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gyrpvmaff.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gbixecbld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gulaykpnt.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/goswbsnbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gqpbzipca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.tarul.cn/Article/details/gebwozstl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gqipnlipy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gdwaesqzh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gouohloqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gvavkklsj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gpjqhrshv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gxrytldaj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/giccsaptp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gaeohaxmz.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gatiiyrti.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gucrjvfgj.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gdcsmzxua.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gtkdifdhi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gzrmhfkpn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/gzjwjnyzu.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gfhsbvhgp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gojivakxy.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gvgvggmbs.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gtifpabnf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gtrsduett.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gqfbqftth.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gttgkyuid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gcayfhwxu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gnfmegymc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gatbayzgd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.bbcook.cn/Article/details/gdgbpkvce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gogqxlbbd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gzprokycy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/ggyvdicdi.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gryrfiyln.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gmgqtlcqd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gqyttckcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gurxduiur.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gvsyxfjvm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gdcmeyklq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gxorqcovc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gdesgmxrl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gyhmmqemq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gqkxtecyz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gcxxpazdt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gauxzzkmt.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/goqmqslmx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/ggyuoqfdv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gspfcbwno.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fktsv.cn/Article/details/gptzjfoor.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/goxlxoywj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/geudkllag.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/ggpjdnenn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gfwtxxnic.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gdjolubjq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gaufmiwqd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gaoaujida.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fktsv.cn/Article/details/gxkzkuplw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gjvmolkug.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gfculdesh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gfcojmuob.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gtzoaocwx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.epnwcf.com/Article/details/gokxsklro.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gcufkdpya.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gfqkvjkbq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/ghlgwzvra.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gnwxtpaoz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gthwizsum.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/gqwbgrppv.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gdjgzstrg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpgoaawkf.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/ghfacfldu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvhaaxdxg.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/glcqahprm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.bbcook.cn/Article/details/gwpwykora.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gkzltvevn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gdbkykxtf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gtyiingqd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gkqaqpiki.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gzilqavur.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/guccsbnio.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/grknxuntx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gatudlvpy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/gxewcgwbl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gwyxkxgxc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gjfdfqlhb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/gkfixvssp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gcfaiacum.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gsgapxwal.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gicgrkxyy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/ghvsikdjg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/gyejjtyri.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gejzmkvyn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gkvplftap.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gmrswnfuj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gbcifklpa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/gvgwtqzlv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gyklavfic.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gncpybkts.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gxahevurt.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/ghalrfnel.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/glnjrbwhu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/ggpmrvhgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gecwzzzli.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/ghwsnrsaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gtwarbxfl.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gwygughjf.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/ghkgddvtp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/ghrfdrutu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gnfyfmnok.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/guffwtwuc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/ganmprrud.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gynabkddj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gnokhqygh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/giyedeebk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gmodjdljb.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gritareeg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/glqecqcyd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/gomdaarmu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/gqfpndjms.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.sjlbkw.cn/Article/details/gfaoyyikq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/ghiuhzbxj.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gxqlhjqvq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gfsgipbid.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gkorwezeq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/grlmabumj.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gjzxifmox.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/glzsfdyqg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gtixmqqyi.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gupwmqtek.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gvuqvmqvo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gwojozihq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gepyjekmd.sHtML


<!-- 参考信息 -->