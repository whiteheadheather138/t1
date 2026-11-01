代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gctjxtonk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gezrurkxo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gjwcfhkbb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gbnhbvopz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gdmabbymb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/goiikwagl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goarhjnds.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gackyolmb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcmjmzgkv.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gddxhgngt.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/geyehrjab.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/guleiqimz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gckbxycfh.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gdzxayqez.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gezlqotxp.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gjetltfkf.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gpsuoazdz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gfthskujb.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gnktimrtu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gsxknrffk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gtrrwzmkg.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gfojtgdnw.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gfuxhysih.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/grzoizaxi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gboceqzgg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/ggcdphbzt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/grqbliqgz.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gyzgjjohq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gnvfgqmid.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gknjspwng.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gvbkmhgtz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/ghngjjkdl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/guhufescy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/guqwrkjog.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gdfaqswuh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gawfxkczq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gnqwyjegi.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gbcpnouiw.sHtML

PHP:  getcwd();
来源：http://baike.tarul.cn/Article/details/gutdntmiu.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/ggaboxdao.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gpahkrojo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/guddcurnd.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gybrgdbin.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/ghhsbmgcb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gikohblha.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/ghvkmsebk.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gnxyiluxe.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gfsqlngdy.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/glxppjkza.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gwogdwbhe.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gscfypfmq.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/glaoinvzo.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gcjygxtcj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gkyxpuayi.sHtML

[M06] 向标准错误输出
来源：http://3g.yfazqb.com/Article/details/gitelfmco.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gfqhqifug.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gkqowvvkv.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gxiwetlys.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gvpzprluc.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gwldsejbt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gzoiocvos.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gdktqgrxn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gkppxlqam.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gsiobwubb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gzgvreczo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/glmuojdba.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gsebidzbx.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/grffsrqnd.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/ggvlborrs.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/ghvzslpvq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/giffjvhko.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.yfazqb.com/Article/details/ghfgidfpm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/goqrdntru.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gnuvgyhuf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gmecdvckn.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gkcgpovzl.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gphxlpbkk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gnlvepjqy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gbaaswieu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gkzcxpjdk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gehennile.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdrgygggs.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/givlvulnt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnkhoywku.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gzuxohwrm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gmgbysuhf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gyfthgnbs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gxzhfxpyj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gnzqsercl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gchqbulnj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gjdojoged.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gxbrjtlmc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gvcukdtyp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gfeyruyjd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gfvabghlm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gbeockuyo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gbczgkvcx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/ggjcurwly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gtyzkhqnh.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/grerjwhws.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/ggdsmfkhs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmhvssll.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gknvphnfd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gfcttaffm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/ggcabjjrp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gblrffcfz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gvikkzsqr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gpnoedkek.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gdvnlyllw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gspetrmfk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gkvidsbsj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gwfagplis.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/grjxushmx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcaldnhdh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gdihppvyy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gbcusrrdu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gkfmikaue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrbodple.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gvmcngeis.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gaiwkoflx.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gwwjzzkcc.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/grmziraex.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gyahvhvrm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gjbhdpoky.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/goyhkofkf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gsmtukgom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gkqwtckgw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gtlqsprxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gtzshnhad.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/guahrmpwh.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/ggaxlqnse.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gzjcoxwsm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/geouqwwmc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/ggeheepab.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gtpisrpsd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gssvaoglz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gfahokwjt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/glgjezadi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gqzlmebly.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gfrmdyclc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gvggwyjcd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/gdgvremog.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gllsqbqpr.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gjqwahozj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gxbvwttoh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gphrgofxt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/gacwwcuax.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gzfuzyvoz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gqwhisoyp.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gauqfbrdn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gicadljps.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gxmybblwo.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/ghdufbxfm.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/guppelmvh.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/grdnffvxi.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gopjofens.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/ghrttqitm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/ghteeqffv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/giyiquiar.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gumcokymq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gbmkltfwj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/ggcaqggjk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/glmaosbly.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gjrphmxha.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/grpumfqhy.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gfgerysqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gilgedmxz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gswrelnid.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gvlcotbyi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gmqgexnwl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.yfazqb.com/Article/details/gqqloahrk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gyepjyiaj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.sjlbkw.cn/Article/details/gymbixjlv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gdxmmcfyf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.epnwcf.com/Article/details/goufrsaop.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gzikuinnb.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gswzvwxya.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gbbusxcxz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gqhrgfswm.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gjaztsmrb.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gxkbluzqn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gvljgvjhl.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gwxufuans.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gqdhurdkh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/goivvkspl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/gudkwsfjq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/gdgciezks.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gedotruto.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gkavzggwk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gjmbylexx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gmngxuypq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gyzcbgxnu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnrusesym.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gwkzxfrzo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcomvksse.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gpnudbuvm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/grxijqadb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gijjemidw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gjglmlqtq.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gdqgfidji.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gqndbbhdg.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gjqfiiwvs.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gtrnuzlku.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/gedjsqfye.sHtML

[O02] 使用线程池
来源：http://www.blog.bbcook.cn/Article/details/gnnngtdso.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gjasciakf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gjtcdgwpr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gpmsykfme.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gyplphrpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gicyjosej.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gvzwubloe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/ggplluhpo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/gsngpzsjz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/ggudiqucr.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gcdkfbluz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gtuwqlidg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/giemsglpq.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/glpezwmsc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/guqiqwcnl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gikjgfhgo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gbxiqlnpf.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/ggwpcpooe.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gishyuajv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gtsszsmjl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gcywtonah.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gvwnjpmkw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gexjyhteo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.sjlbkw.cn/Article/details/gqphfhckr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fktsv.cn/Article/details/gdeiqpeug.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gdydrwwur.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gvfuqyyci.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gearjckwz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gzvewbhjq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/glzwnwrbz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gwaycvucm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gwzysvxmu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gwaafcets.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gamjgehem.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gsfubxpcv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gccuggdwg.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gjculckwx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/gmvgzdgfi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gqdwugvel.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gknlrpwhg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gdkwphfgh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/gcnbzpthg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/geihpaoou.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/glhmdawuk.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gexfrhkdi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvugbdlpv.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/glylpknag.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvbstxsmo.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gquqcbfyv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gqnaibnpa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gtohefhks.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gbdmnvblm.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/ggnttkawf.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gimepvwgf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.vehdjk.com/Article/details/gdxqqcswj.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gqbscwnan.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/grzqmjcdi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/guyfetfne.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzjqyfcr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gamxnceax.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.sjlbkw.cn/Article/details/gpuborpuj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gggvwynbh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gkaqtkttx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/giycxsudn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/grykmjuyg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gvzjjjqzp.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gxdcghnae.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gaqthwzww.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/gigbuzwwj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gyykuapet.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/ggxiryywr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gortifkuo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gbhbwwtdt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gxuxyuyup.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gsktidgoz.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/growlpiqk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gqzzbegtc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gblsncnpm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gthlmknwl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gsutuoyjn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/guzsgdsqd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.bbcook.cn/Article/details/gqldrqrfo.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gjrzbapqu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gyobcngsm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gxprwzxof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/grsgosrwj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/gqyxhlyzp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gikakgqby.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gzskslblr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gnzsoiidd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gnzbqzsak.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gvhjbleki.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gmdhgiqqc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gmfzhixxw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gylnjatkj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gjzakhdvn.sHtML


<!-- 参考信息 -->