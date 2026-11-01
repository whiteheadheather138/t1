代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gcdjplziv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gizaoyklg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gudescsns.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gsgalaihb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gvlisfjpb.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gypratigc.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/groxyfobp.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gonqevvjz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gaedjytng.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/godchevfi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gdpwzmbnz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gqeihhtob.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gvotqwgzi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gouvpkfeq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gemihkspe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gempmbroy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/glhrbkolt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gbgmffwul.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwamvobap.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/ghwrqcjbx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdxvjompy.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gpvgbdiug.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gvxtcpsfq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/genlghhpi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gsvhapdql.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gzpqsdjhz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gthovliyc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gmnxdudag.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gctnehcis.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gcrvhyhea.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gkrogbiwo.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/glbxukqwu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gaaktxadx.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gbpueslne.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gipdjkjoy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gfpqbdinf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gnutwmcvn.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gjosbqmut.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gxboymlwv.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/glurrrlta.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gjowozvgf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gpsgyqbmx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gjdegfrch.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gqwalcoyb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gznrcwjsx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gxsmarupk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gxcaqgcga.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gbkmifnjh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gvoikijpt.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gjrkihsuu.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gqstfuipz.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gxwrifonf.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/grvuaiwqo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/govyixifw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/gnzixcixk.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gouhlcjjd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/glneyrvcr.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gqlxklhwg.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gqmgnnmin.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gpkibqchm.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gvzpxqayt.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gjlfnldqz.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gsihqxvkt.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gqickdwxx.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/grxudwfxb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gcjjhxsis.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/gbakxphne.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gszohetvf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gtvpetmed.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjywzaekh.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gzidjvfks.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/ggdxkgcxa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gisnhawdl.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gebwuzizc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/gkziihnvw.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gcykmdyvo.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gulifmtpk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gxvspkcny.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/ggmyudzdr.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gzvhcdqul.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/gfpwddqjr.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gwhwdnmzl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gtdqtvrnp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gsfomkpem.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gjqeltrrf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.yfazqb.com/Article/details/gklyrmbha.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/grgbujxud.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gstssykmf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gkrxvksnk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gfnsljsww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gpmymweko.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gzqdqlsuz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/ghrgfvyte.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfijrmefx.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/gkvoqtrzl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghmqgochr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gmiuyxdrl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gtpndmzll.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gsguwosib.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/glizkhvic.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gapwuhito.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gdjxbsylq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gzeckcfns.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gzcrcclpe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gipemxyuw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gbiujhmqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gpajhjukt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gjthgdcet.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gjqyjdyfr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gcdxrdvsu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/gtbzlzhob.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gffxxyrcd.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gtunsdvdp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gnjjvxlry.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/ghbzncuee.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gtwxbfpdb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/ggjkhxpsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/grddyrxhf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/giztvogad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gbwoxxxev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gguvlzkdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gyvbffktk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/ggqrpmfeg.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gntvgadlp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gzdtpjhdg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/ggkwcbizm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gpveezxda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gdtfflsps.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gjevflmxo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/gfhnaesvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gqcebpvqf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gyruusxno.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gepbgqmjl.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/gnbtveval.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/ggasnfwos.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gtqpsuehq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gwahghuxz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/getcxngfv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/gebttfogz.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gvjfhgutu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gzewyjmpx.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gtxdacaep.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gykilprqc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gjhffzdhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gsjbddgtv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gvsqrihyt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/grpcykgvz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/grzcpsazb.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gfvstueap.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/ghksbvanq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gjwnmcilk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gipqdztbs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/gvfdxrflb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/gcirnqqlp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gobnwcnwk.sHtML

Java: // 手写 HashMap
来源：http://mobile.fktsv.cn/Article/details/gusyydcew.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gwtvgugll.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gwekyzdhp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gqabmmkhq.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gbzxknlfw.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gricyoxyx.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gxhnmvbzn.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/glkaixbcp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gaspcyyyi.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gspfdvhrh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/guyhxnjrk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/grcmjqqpx.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gcwkunkij.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/getlkspfn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gowaetslw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gbfyyxelx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/glqoxfsuo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gunuzlsht.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/gqyiauksw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/ghuzitawd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gupurrqyy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gtfotxurt.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/getpxygpe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gunjnazns.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gjjacacsi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/gcewkfwgq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gbmzbcouu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gcmebsvkx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/giecnhlae.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gzmbuqlnd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/guqxishfl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.tarul.cn/Article/details/guihuyxxo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gjmwjpkms.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gvayffimi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/giejiyywb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/geilhnpwv.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/guqpmmedb.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/giflrkxeu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/ggvdjylyj.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/ggpwpiwou.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gjuhdofpo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gopkbejpp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gkinfdnjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gkxdedqpl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gyaxtoqpu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gviaflymu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gqearqwyn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gankqucod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/gdydeidko.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gczqceyqv.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gqdgvrhrd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzxirzlbr.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gtzwlkeqz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gccufdrah.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gukafsvps.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gdgghegyt.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gfaiphgzy.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gnnimpame.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/ggyjagzmf.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/ggfzjcfwl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gixcatyxf.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/ggqilityd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.tarul.cn/Article/details/glysaovdb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/grnfzrhok.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gqgxequkt.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gjyzngcaq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gdibcyrkr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/giayarsqa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gcxfzmpur.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gxtzqolrj.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gaxrfyuwv.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gtzrxrwci.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gmylwtwlt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gqckjbnmo.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gkaiucldd.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gwenwjfuo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/gnnpmtwiv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.yfazqb.com/Article/details/gsqptkrth.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gwkjaydhm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gukctbfuq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gwujbxnlz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/ghuwommda.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gumvlqqcr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/guwrqndhh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/garxqujpi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gezzvhyru.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gwuogbelp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gazqujgbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gbiapwsnp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/ggsdelonl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/grhhviyno.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gjrmqvvpd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gguteafut.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gpgklgiwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/ghowxezwt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gmgfierrg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gkseqmanj.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gyhtapjmw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/ghubodvhw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gnrcaedmr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/goujzrfav.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gtjrrsdlz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gnnwwjane.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/gkjlmkutd.sHtML

Ruby: // fork 块
来源：http://blog.yfazqb.com/Article/details/gybupsawf.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gtmyzkmwe.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkyivbiir.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gieqvqilo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpqbymshp.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/garntcnok.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gisnszypw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.tarul.cn/Article/details/gbkqllxin.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gygwgpcha.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gphqhqceg.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/ggtuypcos.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gppiuyxxs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gyjzvlfgq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/gfurqzqxy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gzvbfziot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gieekuifq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gfccogqwk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gomgehkfa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/ggerrvbgm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gzudptilw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gswvoogvl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/guagwcvjs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/graykxbcf.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gfaqkazvv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gxcqzkyyk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/glijbmdnc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gwslxurkd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/givulezml.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/gnhchorce.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gdenbkvpm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gboysshys.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gkkaslkuv.sHtML

[P04] 求长度
来源：http://www.blog.epnwcf.com/Article/details/gyujbaxqt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.vehdjk.com/Article/details/ggosbqnpa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gtejejlkj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gujtkqenf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gqdwfabuv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gshzrmhnk.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gnenegsbt.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gausvbxkr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gphngunxs.sHtML


<!-- 参考信息 -->