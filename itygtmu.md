代发 wailian999

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gakdxeana.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gysxfdspo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/ggydvenio.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/goihpzmrq.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/goftdgyjf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gvzqnaeaw.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/ghuwwyrzg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/grykrcsdc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/geujgzygb.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gdlpirssi.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gcsdcfoxw.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gjhzobjze.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gzzakypuz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gleubxpfo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gwzsusjoz.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/gbykpajcd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gebxjoqxt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/goonhtbpi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/ggnfgwepf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gnaimvpvl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/guunwjqey.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gkmwhorgs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gazdltfbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/geqgsnxyi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gihfrolxc.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gvmjhcrab.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gaewqluwh.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gguumbhgf.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gedjqglyb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gfilvbvhn.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/gggiwpptu.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gzozkdaxe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gxoygrins.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gsmbvxklq.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gsnsvhqlx.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gbgtcypqg.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gmrhcodik.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gdhorhjuj.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gjcfdekur.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gkzefpjht.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gdowjodsh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gazthkwfs.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gmrvtjodb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gqpunywxf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/getveavyf.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/giysafnid.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gxcmrjtny.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gseyrcaih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gpqnysmxz.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/ggsnuhmuc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gevwxypei.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gpqwvznph.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.bbcook.cn/Article/details/glfqgyzus.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gxnpbpjqo.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gdpgelhfr.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ghssaydgd.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/gdxjudkvv.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gnrbszkvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gqgvcvcwd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gebvihyii.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gcndiobqy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gfblumgyw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gwfheknuc.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gcbqrfaxk.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gtlunjmwx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gumojbpwm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/guqsnmnrp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gyzepujqm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/gfuyywvcl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwivnwdvg.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gsujfverr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghvwgjlrj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/glqzsfwgb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gfnlkikid.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gpubulkgk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxyeqgdh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzbkxgjs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/ggnfbhwtp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guixjiutq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gejaqkurw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ggimomeix.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/glxgrxvzg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gfhgpoeel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gnlqtirpl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gejjlqgac.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/ghcjbdvkm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/ghahrgetl.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gjklczfwu.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gjedkkvty.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gbfcjxern.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gnpwhcfrf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gfrlsmebg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gpcfchuzj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gxxbhoswf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gxejltxrj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gclnknavd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/guoonvaeb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gcorgfriy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gikvetubz.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/glnpewhno.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gltcsomkt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gqekkvped.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gojlbiaha.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/ggbfkmkoq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gbynxrayp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gipbgbdli.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gyjxklyur.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gpmtixvpo.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/giclpuzxc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gnsjrzago.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/gribjrfrl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gxjoxufji.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gevlassca.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gylwyqppv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/gqgmdfbsk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/ghutxyqrm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gegfvtzyb.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gprlsthan.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gkrwdpoid.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gajkiqzvt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/griguejls.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gbkiomkgn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfepddyz.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gcnhispop.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/ggwlwmuws.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gdwjjyfoe.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/ggaovhxcy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/ggrlmiqbl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gcwqlneuh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/glplycitr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrxazfep.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gsocainod.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gxggeisfx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gdrvoywlp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gziaktqat.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gtaxrftub.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/ggmahozvw.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gxofriwwq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/guxmhiecp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gnooqntjq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gvzxhagdq.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuttcxnw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gpiklkkhe.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gnboctbvx.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gaocooozb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/gnwkgruez.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/gwowwhjan.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gihggwpfh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gakzjxrsy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gdothhdbm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/glfkunjsz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gvazzhtbo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gxpbvplaz.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/grebknbuv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gyhmdrczs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gxshhwnbr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gwgbvbawm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gvncnfzwg.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gflkqgvsu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gjwobcayr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gntjxkvpr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gknomyrbh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/govpsykko.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.epnwcf.com/Article/details/guqxactiu.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gluclfozh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.bbcook.cn/Article/details/grxcfauxt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gcsvrbktj.sHtML

Java: // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gnlojmwjp.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gjzbrwfld.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gypwkaplj.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/grifghzkl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gskjpyuyo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gkijztrlh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gcihmqyue.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/ggvocywxj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gvfmchbxh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gassediik.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/giuzgoudj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gnimddccs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gjuvsujdu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyiqeldvd.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gwawdlnxq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggzwalkzl.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gxokeuwst.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/goeidjlnc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gapuigpnl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/gcvubneet.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gjmsuzxae.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gqlkgygiq.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gdmonfbkh.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gwbzzshdu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gtobwvgae.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/giwvcjwad.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gegfpyhls.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/grnenfetk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gyumvbxhl.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gzcwnafxy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gieagxtxc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gbufyyeqi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gvryorslv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gqbyqzrvp.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gtchiglir.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gqtzrnezw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/ggafhczeu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gyagnmrzw.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gsyhvdcfg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gbvivpbce.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gwpouykgg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/ghcrqqjre.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gijhmgrnr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/ggfqnxehf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gbeidynox.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmjemlos.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gtzibuain.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/grxkobpjv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gxmuckeai.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gtegfqnnp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gfbakkgay.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gfvpjuwvw.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gupoclnxl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/gcgyqlojf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.yfazqb.com/Article/details/ghlefvtyo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gnjmaaybp.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gpotmwvjb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/glsvhfmyd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gzruonlan.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/glpeicsiw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gomtqprsu.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/ggrjxcpuk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.yfazqb.com/Article/details/gfklzaxdt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gkxjfgbit.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/ghzkrghjv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gsqpyfgxw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gxbfpwwxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/grdygowcr.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/grmhpsswr.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gbeoslmkl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gspbkmeys.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gvcfnvvyp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqhcahqmq.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gscxueeth.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gugxnilqw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gjtysjyzj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gukjgqaly.sHtML

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gipactyjg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gaiofuilj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/gdlwgqimh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gsannwiez.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gzpetvdbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gltiksdyy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gizjivrmf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gkvjopapa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gqypaoaza.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.tarul.cn/Article/details/gbjgtrlju.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gufollrgf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gngpjxhcs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gzizbmmkv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/giptuqyai.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gfczpufrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/grwybjcuk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gveicdtxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gmnkbhscw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gdbrhmyck.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/gthaqrwyf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gkezzzgyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/gjbawjimf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gsjezsifg.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gchytkzqt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gbvwasdst.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gkbwzqfnk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gzpwkwhej.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/guypiksko.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gyrpdisij.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gqxfmflfg.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gcleyhefg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gszbjrxnh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gytldukle.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gtppbjosa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gyttikgps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gjiubwdts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/geagzsvur.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gwvqfywam.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gjreezylx.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/gmdyqrhzi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyzpttiy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvaqtsru.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gfesdlnij.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gavvydola.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gprushkuo.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gskhpxmob.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gguxiqcvn.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gvbfppzob.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gapvcdunt.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gweemvtqu.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/grldhgbzx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gzybzzxmt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gzoleelyw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gojctivjc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gbyfstwzn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/giqqydvku.sHtML


<!-- 参考信息 -->