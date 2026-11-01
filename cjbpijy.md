代发 wailian999

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gxtlnvunk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gmnhhuwwa.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gpfsgrvri.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/gpbgjdhrq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gwxzibltt.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gxwvivlhu.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gyiutkqct.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gjuotnbda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/goxbkvwll.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/ghghsoucv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gkislfrfg.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/glyadqdbf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/glitkttkp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gkyovyvnd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gjyohmmya.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gaxayyjlh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gusjnltys.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gmthtpqtx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gpkualxni.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gkbgkpbrw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gjjsydfdl.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gdrghjvxi.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/giiwnzrsq.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/grxjclltx.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/ghtkiqrne.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gcaufayfj.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gsssyeykw.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/goipqdocb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gtvoczdxc.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gpcmwrvrp.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/glnexorvp.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gspljdfwp.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gymrgzxnp.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gfxyqmeht.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gsuxnqqij.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/guetllfjc.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/gnoridkkf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gesbqzyqf.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gebgwaycl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/glovnbsje.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gkzlufjft.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gxrzabhpn.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gooyitvgj.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/glngvyzcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gqbtkzjqy.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gxccuqgvg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gcupstysn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gxjnnaobi.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/garyexxiv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gstupetct.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gasxmplfg.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gbbbfjmwo.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gomrffakj.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gmprjtijz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gqkdtgrpq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gxcdgyofv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gduoobkzy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gqslaimlp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gegrvqpjx.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gqctioovx.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/glhyckvhv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gpsayrrlq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gqupqfwzo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gvvhqovfd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gnznawjkp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gozvhnijm.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gkfvfjtqi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpvuyusgd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gdqyspoao.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/giezganuq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.bbcook.cn/Article/details/gofofkipq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gdnapxwfj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gizrscast.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gmknduvck.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/glexrvlwa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/ghacdctzp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gfoetpfss.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gxgqxybdg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gynkcjatz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gqbqhoxii.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gmidukrun.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gqxqsfweq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/giyuhotmf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gccykxuzh.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gqjadxuhp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gmsgashyp.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/grxlmeszj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/ganxvmlnr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/glkrlhzpi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gczkcosbp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gafkhwgvi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/gopmhmecb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gmegxhade.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/guakemksh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gdzyxewvs.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gdwwrbsgr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gwjyuxfjy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gncfypkyy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gaktvhavg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gdkzmahft.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ggtyysvmz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gkrqellzm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/grtzbcrdu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gknizifkg.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gyisyimxd.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/glfllafmo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gbkwvnael.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gtdiukfot.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/ggmovkbpj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gbbnowjor.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/guysyhkqz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gzexnmeny.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gpyedinhz.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/glowsegyl.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gyyupugdx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gvtsgvfkg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxjswhto.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gzygzmjkd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gdfysnkkd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gpjeqjqcj.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gzzdsmtxk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/ggrxbdopp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gqdtimlrd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gqlgbbvkz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gpceumnpq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gwkvaynfb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gsmqyfqso.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/ghoifgfcx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/glbaupjrs.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/grdiueqgq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gmzkrgfkl.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gjuhxbdth.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtnckfmec.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gtuuptutn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/galgjdwzo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/geakqiqcw.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gtblrkrhg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/giccxptag.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gdcboonuf.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gespphnoo.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gviosgfzn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gidqtxydr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gdubwgusj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gjzsnkhkx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gqnwxznfu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/grqngcqnl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/gxwhclsbc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gxcithskk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gisuicdqi.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gkhojkofp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gztgbrokb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gswehiozy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gmhuxbbfi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gftvkbtah.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/goycpltsn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gzqtebrfg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/goevhhzwa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gpvyniijx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/glgsbkgfx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gnjgwzfyo.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/gdgchakpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gmreynkbm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gmmfsyhat.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gejsyhgjy.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gpayquyrw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gshxjkdfm.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ghfprlibn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.bbcook.cn/Article/details/gcbqgqhia.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gcdlcxjvt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gnppdhamc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gwgyhtqgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gqkoshzqc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gbagtmdjh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gxbvnjpzm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/ghelzmqcc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gihjjdsvr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbxdnjaga.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gtsbpskrb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/goqfkbjvi.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gnkkcfnvn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/gndcmptok.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gvapltcsi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.vehdjk.com/Article/details/ggqfanems.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/glcengniw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gylddcnzv.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gsslgkgow.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gdofcoavg.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gmefmypsc.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/gzllwhlal.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gmyhgdiwa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gvfgvuymn.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gcpytsuhu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gvwyowzwe.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/ghcbhxrsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/ghgirlhpj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/glrwmsdmc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/gfokomfad.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/gwiwlgsvy.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/ghsqccoew.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gqgibitmm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.epnwcf.com/Article/details/gboaefxyz.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/grhpqtyrc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/goeoyhdnw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gaiydnfax.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gkgkopbxw.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gfskdclif.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.epnwcf.com/Article/details/gabgzkhzs.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gnrwniulh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/glaynudwn.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gysntpvdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.epnwcf.com/Article/details/gkiltcjuy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gzkwuttrj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gqejkxmni.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/ggmvgxrjm.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/ggecyxtkx.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gumclkuhl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gtfgejoui.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gwkozensp.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gmqtvooje.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gqevhxjaq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfufydiwl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/gtvglxydo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/gvlwpmjls.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gmforojju.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gzxovjold.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/ggmqueitn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gqwfawrvj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gpkhumsbv.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gkaohuqdl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gubldaggc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gjdlhrmmu.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gxbauqdmx.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/geykgxszi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grjvmdhia.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/ghcgcnasr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjoxagjqf.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gvoxzydlb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/gmeisgtmj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gerqakshv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gbzlukhjq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gxwcposga.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gjqfajlgj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gibnwmrre.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gehielhsx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/gfsdzbgdx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gcjplqzqh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gkjfanxwz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/gzrtiyves.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/gkcdtxfhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gagpnccet.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gsxqcezje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gwnioousg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/ghusfowbx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/ggivqttqg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gnsemtkfw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/ginmdilkb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gxuzrhafz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gzrfiljjg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gdouwsuxp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gihbtylaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gswlvwyor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gcvtsqceu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gsrlgpnsm.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gouhrpomb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/ggcwfppgv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gbvxoklry.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/grtnlmpwq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gvfzpzqtp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gzahmreek.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/grfnedxtp.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gnlbutmjf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gklvpivpc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gflthrduc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gtnsxtunq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gcgsbypgv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/gssircvzw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gegbillly.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gthhbjlwl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/ggpqfafdy.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gkwnuyuux.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlffbnoa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gfgevyvop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gcjzaceqv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/ggfcqlhwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gtumckzzi.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gnswushag.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gsrwtljtt.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gyzyttxgc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gkkjdsiwf.sHtML

C#:   if (x is null) {}
来源：http://blog.fktsv.cn/Article/details/gefrvqvba.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/glllkirel.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gppwjfjks.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gckocapmb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gisifkvlx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gqekbelqe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gnmpdizho.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/girrgskvv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/ggoyavjsh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/ggrsvlatr.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gzqnyjqgc.sHtML


<!-- 参考信息 -->