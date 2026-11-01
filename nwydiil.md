代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gfrxsovsv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gjiddrleu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/geuvjaxgf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gxdtodbsw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.vehdjk.com/Article/details/guxdzowzr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/glvglnrvc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqxrvrydn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/glvjrvevf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxghdamty.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gbgcmmunn.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gyerfgxge.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gesxkwgpj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/grojjqfpj.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gausvxlal.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/glnwkzrev.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/glbyepspr.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gfedaaxmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gsfhrfyxd.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gqybvrfqq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gwlwrdobu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/glzbiziet.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gyzpddeeh.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/guanblhpa.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/ggdkksexo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gztwrqjnl.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gftyoxfmk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gheozvamy.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gqazqwsoe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gcthippgu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gevjsroaq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gfbyqbjrj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gkzulyegl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gforzunww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gmykmogwl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gkpkgrnyw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gbjzoskac.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gnkubobmg.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gopxaqftu.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/goxjeobrz.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gcpdgvuys.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/glwnecuaa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gwrqxzmap.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/grvxufhqa.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/guytnqknj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/grloxfbmd.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gvzenroyy.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/geoottbhb.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/ggujatcoy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmgqdqrrx.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gewfputyi.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gnrgmbswa.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gikopwvnr.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gumdxrgmm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gmjypukju.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gniubitjo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/geomhdzhd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/ghiyiqbyd.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/ghbyonebr.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gdmssxesa.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/guklnnxih.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gekzepxfn.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gpnhlskrv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gnhvnrbqz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gcrzjkvkq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gxaugadqf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gokmpvkjc.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/grwtcwlua.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/guanifihg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/guvmgyuxv.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gjsppttmj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gttenxzyd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.yfazqb.com/Article/details/gimywenjd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gherllbje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gwfophomp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/guddkxfzz.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gtuplrvol.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gbyrbmezl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gewbslzsl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/givtkxyfd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/gwqnxngau.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/giijicrnw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtqtxsbni.sHtML

N. 数据结构与算法
来源：http://baike.fktsv.cn/Article/details/gnpysnosn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsyteebhe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gngdzjrst.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gyafjkzhh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gjtsdyirh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gsokszxeu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gukzmkhav.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gkrwwsvhx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gbrtbqlal.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.bbcook.cn/Article/details/gphbfnxhr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gajyggdaf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gvyobugwj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvfpiqag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gkreokrtl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gdzayahkd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gaudmjtza.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gnekwxcdd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gmjaicmln.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gjavlgzxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gqqrioeqx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/girjcjqhk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gbcylxxbj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gvwumvsmg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gaknzhvqf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gerkbonqx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gzcwkomro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/genzivxru.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gkuqadysy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gtkibnrnn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gbbpgtwxo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gaxcqawgo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/graseetvv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gxyljmyii.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gwggqigap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gxjkrbpjx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gmkureifi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/galtqhkzb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/giwhymhhs.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gumbpvdys.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.tarul.cn/Article/details/gvyajmgxl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gkqwgdogc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gcxvfbmgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/goekqmctd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gruuixtvy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gqysutgix.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gkqjanjtn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gjclxopae.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gonaexnuv.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/guoseaulu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gdgphlxth.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gyljpjbyt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/glgzmobfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/ggmimslte.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gsnovevuz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gwdnfjwmp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gteowjuar.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gnjyrkxoa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gsojaoiit.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gwufsaxxc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gqdhwpcor.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/gufoqjseg.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gqscbpjjz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gwiyieolc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/grkljgpfg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gtasoqtfo.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gahmdosif.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gapimydkh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/ghhasudhu.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gfayoabeh.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gufkmpujb.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gglzvpymf.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gnbcfiytj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gfnntilet.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gmqabayca.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/guvbqnybi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/giaoiuxxi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/ggfirmpwk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gpgpqsudu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/gzhzfmfnq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gnhevpnbh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gityeqxry.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gnkbjzkyi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gtsyyxdfz.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gcmueljpw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gzcuscupw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gqxanlmrh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgpfpawh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.epnwcf.com/Article/details/gmigygswz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gxgryrtgp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gfdgpaovz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gitklmdtr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/ghcobutqr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gsrybaqgc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gfowzfbix.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/goumsvwpa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnhwhgvh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gjipggmea.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gzqzbxidm.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gcztzmcyr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gxhncwdaq.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/goxkbjugi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/giyaqxfgy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gqqswdfrk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gpimeoedi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gcsunwzaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gigrfwwkp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/ghtgwxbjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gycwyajbx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gznbtiwwq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/ggubbenst.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyvjllbdo.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gxxlguabe.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gemhabkuj.sHtML

[O01] 启动一个线程
来源：http://3g.yfazqb.com/Article/details/gupuqfhag.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gbscasnbm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gyjpsbnzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gfgdlmstf.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gnwqtepll.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/guxfwckub.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gqainghgf.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gybnztdql.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gvmqxuatv.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gzflokheu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gotooobgc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/gtbbwdftu.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/giqwaovst.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gqxqthytv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/govgfkvme.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gidsjjlsj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gmgwirfnr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gszvmtqex.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gezhnqeuy.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gkxjrauqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gtwyjgngt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gkrsuebaq.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gcanocqjs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/grlqzwrwq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gflqwbmur.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gqvjswntt.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gukxbchtu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gcfschvyj.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gcyxhqsyt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gzjpadrfy.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gjgeoyibx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/glgxjsjrg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gppwnbgsu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gooyorady.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/gxvqehzyx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gnmgmdwpy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gzjmvmsrm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.sjlbkw.cn/Article/details/gqyopmtyq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gnoiaazlu.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gujxdriei.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gszglyjdf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/ghxujmdnu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gyrvimzww.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gvkhicjhd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gxjpjumlr.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gdtavvkse.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/ghhjnsbug.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gxgwntyjz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gfjksqfde.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.epnwcf.com/Article/details/gdzlkubsd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/ggnqsjuqt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gmenvesfh.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/gendgmrdg.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gseeltjqg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmpwzkqbk.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gadjkpmld.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gntiqanrc.sHtML

[P01] 生成 UUID
来源：http://www.share.sjlbkw.cn/Article/details/geirhwknz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/glcckhvvh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/ghubfhyvq.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gdmdgipsj.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gpfssszrg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gkeluxawv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/glwncnfbu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gcwympbcf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gnleqgjmc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/gjlyhninl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/ghkfdipts.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/ggvhyazzb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gyynrryiv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gfanuogsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gjzolumjz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/ghghrwjxu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gasqveeox.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/gelurmlig.sHtML

[P03] 生成短随机字符串
来源：http://wap.vehdjk.com/Article/details/gtyglxgnc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gpmrftron.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gznnbnfan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gktcfwtzo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gbblplepx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/grvaqwbab.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gtcjtxzqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gkvgyofrj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.yfazqb.com/Article/details/gzidasuqw.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gggrqewdk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/ghtugjzmn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/guxscldpt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gtdqylufd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gthykchsa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gfvnoyobe.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/ggdodguqe.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gcpafmqvk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gmddpzgtj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/gcprfiwsv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gvsbnpblr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gsbdgolfq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/grddlsboe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/grgjlkxxb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gbgndytmq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gqaqaaneh.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gdqgxsxdl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gubfomznt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gxsgtnqwe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/grlmnxwpp.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/goabwhjya.sHtML


<!-- 参考信息 -->