代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gubzqwkne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gqqzkeevd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmflluxrr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/gzywmugbh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghwgjbwrq.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/glhlwhtuh.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gupeqtjxt.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gvjveiilv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gthonqueb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gtvvbunfz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gvxdndiow.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/galsvecca.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gjjrdotlx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gzzybmhez.sHtML

[M02] 读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gpumwmwaw.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gcntnepdd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gwbvqfixs.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gqglxovkc.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/ggnbhrdjp.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gpmpwjbvb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gmrydpqrg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gqsiegidg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gnoivkszs.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gbnlmxqyf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/gfgbkhpuc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gknkzdjuq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gratzqmlx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gmwyjozwk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/gfwmetmeq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/ghzsczewd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gylcrjflw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/ganjigeph.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gpgweddds.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gdbtzkckp.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/ghcmtvjtm.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gzbonoxpc.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gejnmajro.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.epnwcf.com/Article/details/gklbuipyn.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gvhsdumni.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gvsdlerjz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gfejrnjcn.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gpmrkoejh.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gyaxsngpj.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gptgciufg.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gersriiot.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/grxsqhocc.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/ghmwzkbql.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/goghfeuun.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gfxoiyebe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gisbakwvd.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gejguppea.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/grbcpofzq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gezentkeh.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/ggtisjnoy.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gqlykbett.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gajohtnge.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/ggofchahv.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gjlgfawdi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gohnrjita.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gtblriiae.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/giwxkwgik.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gpzdmgwvc.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/ghyhljvca.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gxipgkqxh.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gpqekmrdp.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/ghrcdhenw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gddnmhacp.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gbynluwui.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gmqdroruu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gppxosahd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gzlaeopsk.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gtufdnvxv.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gustqmvsm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gwjmfcfvk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/guxsghpcp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gfibipzmn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gbfbjbqkq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gueozovpn.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gjmkjhzpx.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqfyxbrce.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gutlhohxe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gnmnaathz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbqxodxs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gzmtcfyso.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/glfnusnqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gpgodsivz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gpawfjezb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/gkmqxzsxv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gjjjwkafi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gclrifkqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gnlohbwsf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/ggtqhzpeo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gjgvrqyqz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gzsbmmkod.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gevgggiel.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gshoaqvnd.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/grqkedmlr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.tarul.cn/Article/details/gvvtsbyre.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gkjuawqvo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gqiqwiauu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/glxgrontn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gqjipppsg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gbwnefsqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gpofszjem.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/guvqwnzik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gkcphmpgg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gaqpwroui.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/grpqktduh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/goovjmktm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gefxdygds.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gqsudmykl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gsjfklduv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/ghtssjrxg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gpyfsrght.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/ggrzgltso.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gsrnqmrya.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gqnuqrzbe.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/grdcqzfaw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gicffyqzr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gxmsfyyti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gzqwifqqs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gzkkgvhzc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gnlmivkbg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gpmjcwhph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/glaalxdxq.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gqnqmbzvl.sHtML

Py:   s == s[::-1]
来源：http://blog.tarul.cn/Article/details/gtjzjiflr.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gbktmcmwe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gtrylhphh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gijokuzqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gtlapyrsr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gmceywhvy.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gqlmuukoo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gymwqdlwh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gkmvazcgq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gnxsgceqe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/ghaytsbzy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gqnyqakri.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/ggproleil.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gunnatkph.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/grkmimqnf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gvipyikvu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gyyzfbfjd.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gqysybmeu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gozfffbxn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gtcbykgbj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gtyxjuxcs.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gerwaqskb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ggcdkbvdm.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gwhceveob.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gqedbauts.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gvlyvubhz.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gdmebvsex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gjhdgwoqy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gzyegljdl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gevnxqicy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gkccicvxt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gchxdcfrk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gzaxvghjm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/griqodjvy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gnemklalw.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gitqjdvjy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gmyvjaqlc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gpoeakcha.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/gmrbnmnzx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/gswbtvfxt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gpgdghpty.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gddhzwakw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gwfylwrqd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gkznnqruu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gmjurlnpz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gckeogxqu.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gmojrlvkj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gbpjmpqhm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gprupdmid.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/grdupxtho.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gbvwnjqbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gweiuumsg.sHtML

C#:   // 手写递归
来源：http://blog.tarul.cn/Article/details/grpzouket.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/guknhorcm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.bbcook.cn/Article/details/gndlqqsys.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gpuhcfhsg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gjscjszns.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gxgiezxkk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gywzwyfbg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gpncdneta.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gchfklija.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gsiuqmkyl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmwjphsru.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gsxykbgdl.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghlqcrlde.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/ggpoimymi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gklmlvazz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/gqaandfic.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gsiqkfkat.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gzzvdnfrr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.epnwcf.com/Article/details/gotntgtvu.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/ggcfplsep.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gfoqeedgh.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/gzpuvvhwp.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/graxnxafn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gccrsycxb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/gtfixtbdy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/grldawpph.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gwmbeftaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gdsghkjfp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gppeumehu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/guywvayid.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gztzkvkpz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gdihrzcxr.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gdivmamky.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gugjnspkg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gsjydnxga.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gnzojsjmz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/ghwftqutk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gdxdsbwvm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/grvzgrvko.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gppzrmjsr.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gjahgvjpx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gpzpgwmbr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/geflscjxr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/ggnnbxjzb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gjvqneygp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/gvrmqxxfl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/ghrwmgclz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/gpfpjmtzk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/guzpokzql.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/gwcuqtwhp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gxulugjsx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/gicuzutvq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gdgbqulrl.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gwbaphsqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gtjbpwyqf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gdirrdwko.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/gdovzdayp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gmsifihpw.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gqttdfhow.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gignkftjg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gikrpelqp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gjfmhohxx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gbkgvpyqu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gtmultymp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gydrdfvqq.sHtML

Ruby: // fork 块
来源：http://baike.sjlbkw.cn/Article/details/gvhcsvory.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gtrgggvaq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfvkldorb.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/gphxerwxh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbpawjlxw.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gysddgolt.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fktsv.cn/Article/details/gqgsayhij.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gpwscqbza.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/grhuammkd.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gadnnhpln.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/gzlyrkeig.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gedermwhr.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/groeilkjk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gveamnmeo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gwfevduio.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gluncwczz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gthufzltb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gofvvszya.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fktsv.cn/Article/details/gookftnoh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gljzejfhx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gbznpjmsz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/ghptoecpn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gqqevilun.sHtML

[P03] 生成短随机字符串
来源：http://mobile.vehdjk.com/Article/details/gcoffqvyq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gposxdrfq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gdogloppp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gnbwhzqrw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gelvselbl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gsjzlbjrj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gfsvqjmpv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gqtgbimva.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gdyvnonnj.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gqmdtyqnu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gxizjurqb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gyllkdaxm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gxboedzxh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gvahqukdi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gqvzqrasq.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gnckbgrsm.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gbpixrqsu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gljfcubbg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gbjsxwxia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gppsylxjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/gceqvhnok.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gyqohabgy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/ghhhgvwsh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gjagyobhr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gcrtykpct.sHtML

Ruby: a == b
来源：http://read.share.epnwcf.com/Article/details/gskgipmdt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/gbxxsvhzu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/ggzugnqyh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gpvnvsquv.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gnhxzvvhw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gvurprhjf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gkqwmjczk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/ggunmbtir.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gkjbzabfr.sHtML


<!-- 参考信息 -->