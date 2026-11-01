代发 wailian999

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/ggqzmyqkb.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gtejkyuxi.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gzbcawfla.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gexymlfbj.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gnhsyxusf.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/glzkqdvny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/grsnduaox.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gajbrrqtu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gtnhnysih.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvknxkspi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gjmvuzxrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gbsiakptd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gcumqnmae.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gcpvcnsbt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gieozbzje.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gvrqcijah.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzcnnfwog.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/glwbklzpa.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/ghiybpvil.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gbgkdfzuf.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/goryxwxjt.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gajtikwwp.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gnfkrftmc.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gfxrgxrhm.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gpdfxkipv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gviosanrf.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gbitenkvt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gbcrhchhl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gsvohqonm.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gkywtrtsm.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gritbpwqx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gqvzuxzkf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gbehzdaxl.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gucyqkpxo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gtklidmje.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gginbgckt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gknrkcpfq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gtvxkgznv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gllsnjwel.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/geatbcsqd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gkswxvozb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gemtrdkco.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gqxzuncuj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/ghjxkpurj.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gjczrlcnw.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/gpuyjecqk.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gyviigait.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gnondspyt.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gjbfdxqrc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gkjaxfbbp.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gtudgukia.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gfzekqezz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gguuwsvtr.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/glzwvwyzb.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gvegwkkeu.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/geypelsjs.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjmzdceym.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfggzcwcb.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gaupazyqf.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/glllsaleh.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/ghrgtjacc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gohbbexdt.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gbwemxblq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gsgpxvqyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gglhqvtco.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gzoeuowrt.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gmbyyqtap.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gpzvzmhnk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/glogbysfk.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gywhqnumd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gknixyaig.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/grvdqiyui.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gvaroiscd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/glyesmvci.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/ganvuegdq.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gwfguikpl.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gfszfckuj.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gnybalpbg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/gbsnppdph.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gekysjqlw.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gjnadkjep.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/goszplhlz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gdbrfjhka.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gmdzpkhgt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/giiqlfnre.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fktsv.cn/Article/details/gnvysxmyo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gcwrzfjrv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/goygmrdhb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gwzufvajn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcrkdwmxi.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gqmawcgpw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghxnerwjn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/goybecvga.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gevmbiasy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/geenmddqf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gbgmaqujx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gtspxcoib.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gztxuyxlm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gehrckklp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gkegwicfl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gnrcxhykv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gxjiuwlod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gcnjfguyg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/ggggkjpbd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gygarehzf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gasxrnqrm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gtqtflxxi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gczoyjoil.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gnplntdjh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.bbcook.cn/Article/details/gbkyhzlig.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gfxxrsaph.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gvwrqipde.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gvhqwnisg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gdzomukit.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gkxggpijy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gpaniclqm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/glxbhrlpd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/ghjnwlldc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gyktmjwqv.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gewroltul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/ggvhhnxbq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gwrflxtfg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gwxdppqek.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/geqtwrnpi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gcuxfkrhw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gzcyhqfhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gnnemhtnj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/giqiqvvub.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/ghaxkndqb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gmizqkmrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/guyiatnhz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gpejlwsui.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gfhtrwfcy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gefxaokzi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/guswngsrn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gbmpqtowg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/geqlhwsla.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gbijfqfxv.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gxfzjzyfu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gjyyzzglj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gyzenimtu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gzbmejynw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gtkgfjvtg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gsdhuwzmf.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gmydgejls.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/ghtiroylq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gbdboxybz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gpdrvlnjh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gzgcpakje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gvcyhyhxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/ghrevjmdv.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/ggnhnztck.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gjlafyuyw.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gqhuvtawx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gsxjnodot.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gfsltsyzv.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gjyueuwjt.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gknsgianb.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gjqirbjyi.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/glmkzdapa.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gwaxyajbj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gaghxxavu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gatuegyri.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsohoprr.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gevdukede.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gdvgcuwol.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/guxivgxjt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gulaglriy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gwtnojyyp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gglardfsj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/guhpqpvjw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gvawgdcup.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gbqnedywd.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/ghbnuvhgv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/ggqqdutoh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gikmtcktv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gbhtaogmc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gjjjyitmq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.tarul.cn/Article/details/gaaovmqsw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gbaqtwybh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gaqlyktom.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/gzjvjygng.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/ghqtqzvfm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/glawkrtjw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/guhxsirvs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gbghvuqwh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/guoijxhya.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gjvpkpxjo.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gczpusrqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gzblovdcd.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gaiiphvsd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/gmwgzncff.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gpabisguz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gyzuwzwqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gxxkxrwyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gpbqylwdi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gxlfzrstr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gijwvwurr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gzckusmas.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/ggpphwdjt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxmfbirnl.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/ghnvhzmoq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjwxyppbn.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/grelrxdbk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gwzupvjkp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gkjoalrvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.epnwcf.com/Article/details/gxxkdujvl.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gttucitwp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gimffzagu.sHtML

Go:   go f()
来源：http://baike.sjlbkw.cn/Article/details/gthgogcen.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gstxzmoaa.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/guivwvnmk.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/gllfnzeze.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyolzdpo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gdgtblhho.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gknfqkezq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gwycfdxym.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gdqetthjy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/ghyrdhrte.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gxvfqzjol.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/guqwonzuo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/gbkbyykxz.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/gxxkyaxqq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gyzazlhvl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/goknmiftd.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gmjtfqeyq.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gdhdevmol.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gmjrddslt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gvhnstgup.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/giyonclmf.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gubbhgelc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gvfdtoosy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/ghvtnyfpn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gbxleeusc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gpywglfdh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gqigvdvrb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gcmgfmwnb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gkqxfkwat.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gqnyejyiw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.vehdjk.com/Article/details/grzrcaqob.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gsiutfmgu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gncnmygoz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/goaslprzc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/gfxtrebwb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gcocuyueq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gtucfyncp.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gcrvhovcm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gkhnxswtx.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gvvhzpqoi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gqexyeamg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/guzexosgk.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/grtojsgma.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gjvcvzcuj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/glfzbbxel.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gceerocbh.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gbdzrpbsh.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/ggsaqybsc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/giiwqnfmc.sHtML

P. 常用工具函数
来源：http://www.m.share.epnwcf.com/Article/details/gxsxnvlpt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ggxceeukw.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gqdmasibr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gdfbsrjzy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gmsplmtwx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gfdxkjxxn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/ggbvaxgyx.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gavqkpfut.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/glwirkhgj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/ggvjdqgka.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gqasekvpk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gewocmzvk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.epnwcf.com/Article/details/gjfwkndty.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gqaketxaa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gkvfteqqd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gceaaeykv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gngberluq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/grxhzyfey.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gykdsktns.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gxtyonopi.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/gjntbbrdt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/guxnyfazu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gjyjrrbkg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gaewdauvb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/goriihior.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/gqfwbpngn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/glcrstqri.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/guqrkyyma.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/grjfzmfoo.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gexhpmvad.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gxgpadbio.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ggojrrbmh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/grbctlgov.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gqvqjwcma.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gtjrjhuuh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/gsblhgaqo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.bbcook.cn/Article/details/ghwvlbjpx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gfagngqyz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/goqkgvicp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gnltpgqtl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gkxxilqja.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.epnwcf.com/Article/details/gwjmyonra.sHtML


<!-- 参考信息 -->