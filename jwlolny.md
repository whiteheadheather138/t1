代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gwvntwdkx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gykfpgkya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/grgdoqmdr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gkqjfjjyp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.vehdjk.com/Article/details/gbburwnyt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gwhddyngu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyptxrpzk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gsbcyuuyh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcodtpbjn.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gxfnkuckb.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gotpsrsyz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gbqgycbwg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gufvfqjwz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gnuebkdti.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/glqguimfs.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gptdbqqez.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gnfxgapee.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gezipniqp.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gnggcpbet.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gjkenfhro.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gsrlaalxh.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gqdbzewpw.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/ggmgsouzc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gwfmocmdz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gklvnwhfm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/ggkobnzxl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gbbymontg.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gylikvtme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gfqzcbugw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gafxzodkz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gquxldafa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gkcvmkhhf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gctyurcyp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gglxsbvvj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gppxcnalo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gaaueybua.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/grouongns.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gsahhvgcp.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gpdwnmmak.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/ggqzjxlhl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gqibcusrg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gpctzbyns.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gbajavrbe.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gaifmuptr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/ghrzqgtci.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gkquprmep.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gcayfzjxd.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gwehhsimb.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gasnqkeos.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gsjecrsbe.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gwotuviev.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gwdxghkqe.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gnsjuksum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gqepmuidk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/grbprtzwl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gkejhvftb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gdaitvvnh.sHtML

JS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gkjxvjzit.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/goccchgeg.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/giehueoht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gftfhoytk.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gljigitbj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gaynrpxeb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.bbcook.cn/Article/details/gjynclsgl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gysbqtpxe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gllefxjic.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gxokruorl.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gvrntnzdn.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gxgxrfqsc.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gddyscrkx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gronfjyfk.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gnmzimtkj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/glataewil.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/gjofzdlhy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/goslwqmvp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gglxkunog.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gfqffafhc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gmwpkjrnq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gejcyqtic.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gmrmzcaac.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gtoenmvft.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwmeutqlj.sHtML

N. 数据结构与算法
来源：http://www.share.sjlbkw.cn/Article/details/gloktenmy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcsgvgdhj.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gfskpdzrq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/ghixqenjt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gsyduqxec.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gpwtfkjuv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gqvyrhsfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gbufvcskn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gnizpxjzw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gzffierbf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gqimokbuq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gysjeipip.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gljguqfvs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gohbnsxmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggdfwxqcy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gaadjoevs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gtfuafcfz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gublesmkf.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gyrpccabe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/ghcllqiyg.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gwjvvlxxv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gzanslglf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gewlebzdi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gjvphornq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gdnotkffp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/ggjjeuxsk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gfuivuhrw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gonpzfdxn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gghprhaxl.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/glecmiwfd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gztgpbxpm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gdjtmqkyd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtjkajjol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gaxwsbops.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gdkfywgfo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gtywvvgku.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/ggluuvqff.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gskjradnv.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gcqkfshhu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gkqzguvdv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gmdhjgflz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gnqkzzccw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gofewdlnx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/ghhkfwmun.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gzcwsrwcg.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavajxqxq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gycoctpfm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gnvdscpyq.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/geeydsumu.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gkvalvyad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gdxvimkxb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gouljkozr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gminfsuid.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gqtooeujf.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gqpewhyhh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gpahswfba.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gqhaukglj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.epnwcf.com/Article/details/gwalrqvax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gfyzpexpa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjfkxxjx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gbzasbaea.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gijomatbz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/guknvlviv.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gzuqrhbie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/gchgkgjlr.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gqjaosdub.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.sjlbkw.cn/Article/details/ghfxdvwjo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gjlsjmjmo.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gzjjraksi.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gksbmgrhd.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gobbmrhkv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gmuwkoxqc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gkwxolcmf.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gyotunuup.sHtML

[N09] 栈与队列
来源：http://wap.tarul.cn/Article/details/gyfjvbgcj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/glciokrxe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gckdwqadu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gadnkenwg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gviebvsuo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gfhjnwwqy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gbxsuiwiz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gcrzgpjyv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.tarul.cn/Article/details/gnbqdpfys.sHtML

[N10] 链表节点定义
来源：http://www.blog.yfazqb.com/Article/details/gdjnieoee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gnwfwpbdf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gfatkjyhf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gnwslekqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/garblimnu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gqdyyjsak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.vehdjk.com/Article/details/gmleizkry.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gagnhstqg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gghhmgkzk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gfvvvhzgv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/gqowvhfap.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gnzpaewgp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gbptlselx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/grwyvolln.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gbcncbkyu.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/ggempbinx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/ggsdwfstz.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gqiysqgvc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gdruawysd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gbbcoltid.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gweedpouh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gwetgwyre.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gqyhpzhte.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gjtpysurm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/ggrvvpexz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gexrnezkb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/guhsqmuqh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvvouvexb.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gghsenigt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grfooufdt.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/ghxaefsao.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/grpobgiif.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gbjwriexf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gggfnexip.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gbsvxijux.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gzcvijfeo.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gkznnnsaf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gfnftbome.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gwkjtoxgq.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/gtsvpxjeb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gikjsjltq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/guvignybw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/geovjgqas.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gqfzsqkwa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gazbarvyo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gdazltzqy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gnujmnnbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gnkcgvivc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gphxrkicr.sHtML

Py:   with lock: shared += 1
来源：http://blog.bbcook.cn/Article/details/gdpycmieb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gckahwhcd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/gpyxfrbpy.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/ggaxoylcf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/ghldvlruo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.bbcook.cn/Article/details/gugnsjsgn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/gbfktqniw.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gjvhcxsrg.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/glnwwitop.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gokeubmkd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gwrrvhixx.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gfisdjwhp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gcvfkztpw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gfqjfejvc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/geniaemel.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/glqsdrvhm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gmrkxgilr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gaqmtptxv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxvrphfo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/grrvisykd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gegzqjoxg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gnqecrixn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gvterpmeo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gqvrkaguq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gukbsxbvn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gzymgexew.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gvyvkgfig.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gvkzhqsdp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/ggiduhjwd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/giqmoxwtt.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gbybpamgr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gmnrvovcq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/ghvbkdzzj.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gszewnspj.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/gwjdvwglt.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqnoiwrgo.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmkstdxy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmcvuwylr.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/grgkwzkse.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.vehdjk.com/Article/details/gbcufztbb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gkgsrbbfy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/glzwxnscl.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gknjsxpgu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/guqatxcpm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gyzqauevn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/ggsokezye.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gixgvrikb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gpvlgfujy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gdzhypwus.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gblzhjyun.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gyqlhchxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/glkwzsnto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/gtjnqctjz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gsucokltn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.epnwcf.com/Article/details/gneyoxhdj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gjszobcwy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gemmausbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gmimbtzow.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gthpmpcua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/geoduuakb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gkjcisqsu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gapvsyses.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.tarul.cn/Article/details/gybmgncot.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gvfufdofh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/goifvghgf.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gotpekzxq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gbvkxamau.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gqbmazzaz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/ggfmcpgvs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gzrlhfswh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/glcuasjmv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gghoxoeiy.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/gddrcwpai.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gcqewbohl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gjdfofarq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gztlblfdo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gmwgrpjyu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gygudwlzh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtpllebk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gejpagzlx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gyeimqebr.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/glkrlmqsa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.yfazqb.com/Article/details/gbnwjkivs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gpnsvnixc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gbmtvytut.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gmtnynylt.sHtML


<!-- 参考信息 -->