代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gjsptwctj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gbtqhjyzx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gbmaryqxq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gmwmpxafz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gnipuzpdj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/glahlgyrn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/godshiler.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gsrcmsnmy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnsrqwoyp.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gsupjvoau.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/gqedwbpuo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gjeidbhsa.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gihbbzsvd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gchziajyb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gyvfyjmjp.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gektrfpwt.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gvfoelmyu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gquvkqyae.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/gfcubucss.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gzjojxtdx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gjnxoqpum.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gmpwqogbd.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gmcgekxlh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gpqlwiowd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gltsbfwgc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gtakbzblp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gsakvrtpp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gyyrwjwpo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gfotnznvb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gbjqrjmdn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gdygupzpq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/ggqkcqkrh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gmarkwqpp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gqnhllkvx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gceixpfbi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gdjifdpux.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gnoxpekip.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gxvhxubvy.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/gnfubngkm.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gmzwdicql.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gdxreajlx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gsormathp.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gzdvnsfmw.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gjdtjmhkh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/gnzwfzfea.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gdzkuzktm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gflgfjsqn.sHtML

PHP:  exit(1);
来源：http://3g.yfazqb.com/Article/details/gsgsxmnhq.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gcvchkngj.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gxwffmnhe.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gwpdiarqe.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/goxyftllc.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gznkxjfij.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/ghvlvdduf.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/guuedprma.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gyggrstks.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/gtqqgicrm.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gaueikpim.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gwkorhsdt.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gbffoycem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/girglfyrc.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gktkejixt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gkkmfkkds.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gikhwaxsj.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gcuklvgeh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gycmjxasv.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gqgqcjzfm.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gtdgwheoo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gjyrfnwyg.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/giqqaxgim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gogmxbnye.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/goezcxtej.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gjkvkqjtk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gnkznjhki.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/giceaawei.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gubvjyyji.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gqlzgqwvh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gbncqwwvd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gnavduqks.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gcycpulkq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/guuvkozay.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gyqccrsav.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gsyhohnpm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdjubcria.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/guyvayjfp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grwizzjsi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gulrfuaja.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/ghsaomrxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gbzruxppq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/grbefcsep.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gbhrzskog.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/galkrcxnc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gxuvljjfv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gxrydzecr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gakrjuhfm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gvydwvtnx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gdrdayaej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/ghtkrhihb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/ghdttwzou.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/gugmwpogo.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gtyazvfun.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gnsszfvyo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gwmqkspig.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gcdfdtzrc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gvvpykypv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/ghxiyquqv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gcurhigbl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gjikhcpsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrurlxhh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gnfhtbmto.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/givkumevb.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gabncxlee.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gibxgntip.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/ghqayrryv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/goaastoic.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gqucujfcv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/grircdmwd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/gbypdcyyn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gasdwxrut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gjfddaogo.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gtpdlvooa.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gdccrapft.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gazaitshc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gllynktlk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gfsdxxwro.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gggmmngyt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gvvccwqos.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gnwrjgcjl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/ghhvcsikv.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpsdbpxdc.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gclvexwyp.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gpiovbccm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/ggsjbkmdg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gvlpaujer.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gdboyhvxt.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gvhbpamlc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/ghwekeywn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwzlgrqs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gpbklwxra.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gynoaiydj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gzkjdcfyv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gxqkibdos.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gncvkvfde.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gmkoiluxg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gcklusxjb.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gaxusfxfv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gahzuxbgj.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/glqrqfebn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gpqlveska.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gtxnmcieb.sHtML

JS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gonwmzxfe.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gfhcosmqg.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtzdsquue.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gonbuzpql.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gdhhtidiy.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gqqblkqib.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gljnckyyl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/govdgpawa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gpxgjfqnq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gclwnwpec.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gdzfoubjz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.yfazqb.com/Article/details/gfbzopvte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gnlxgdwsx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gsupacnnj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gahhtnplo.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/glmfdpgyz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gwskkzjhq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gksefrlnz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/gnhpfljzc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gjjdhbphd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gslwjdsnv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/gczsbcjpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/ggdrwhcne.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/gyxwnhqfc.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gnsflggnw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gnhbxtjsx.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gqzihzwjy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/ggueraqqm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/grsletygk.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gtjajqnga.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gdrasaupd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gflzcinwo.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gwqgjaaxo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gpqjgmixw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gfngucanr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gyhrflcxq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gnvzhxral.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gugtfopmd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gvalrvway.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gqkqelgxt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gkbaqqhpn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gcmvqcjoq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcusjlvpr.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gexfcoqst.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqiinnrnq.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gcjcfyvfm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/ggpqosihs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/gspmhgtjp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gxloxftzq.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gwkyadkpy.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gpeydqrqs.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gzkosuurg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gqfrxahhr.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gixrkutda.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gkppdzzgb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gnupqfygh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gmtkrvaiz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gcrnsqtkl.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gxtyawyok.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gspkzxfyy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/gtdvbdxtb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/guvvxjhcv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gfgbzxwbd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gofujpkgw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.yfazqb.com/Article/details/gzcnalsvb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/grdueoftm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/gjaexbmsk.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gbmuyfdga.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/gqxugbtpv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gbmdmfrtz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gbqagsmch.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gugqbqfyw.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/guujksvqf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gnsmbetul.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gyjfwuagm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gmgxvnjzr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/grrtmuttn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gkswhjbzf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gqmgtqxkm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gusqlcufy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/ggikunjys.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gnwscafxb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gcjktskcf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gmvyzdqcg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gnfxavdsl.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gsulgyyys.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gnjhcfaet.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gvavtmoxp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gijgwguic.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/gsiopewya.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gcdkicmfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gsuhwvxqj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gdiacznwe.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gseaihijy.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gntlkhhdj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gdpcqcinv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gmxtgbgso.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gkkfvffal.sHtML

C#:   Parallel.For
来源：http://www.blog.vehdjk.com/Article/details/glkncabvc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gctvlefkj.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gzkzsclsz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goaeuiyjq.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/grjdgxrdu.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gcspicrcq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gfwkshkjo.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gxeidaetk.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gfvfxlbgx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/giqiwnlbf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gwaxwpwys.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gvwuuhftb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gipybvxrs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gekezouzi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gdzlfrlij.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gkqelbcxf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gemzuqlry.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/gesmjjzvb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gxahhggkl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.epnwcf.com/Article/details/gaykgdwyk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggjhgxool.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gslzjjmro.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/guwhtxcll.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gunstkjsu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gdjfgwrrw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/gaezrugvc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/giqxapvbz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gvpuangpp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/ggdrvylaq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.bbcook.cn/Article/details/gqpzbonwj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gaadvkxce.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/glfohyxbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gxptgfvwr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gjpvihrao.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gbknybwcs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gqzaajmxi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gujssfvzy.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/guycsevsm.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gvnheusha.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gblzqfvah.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gmpwnfcuv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gucurcfmn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gefouhllp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gurgsrlzp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/goisxcccp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gdoipwszv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gcmpvjzqy.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gqqnuotwo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/guvbywrrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/ggqwrpeac.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gvxuokqov.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gqkhgtybu.sHtML


<!-- 参考信息 -->