代发 wailian999

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/gatqrujxg.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gsahxxnbt.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gvnxkgujp.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gwsamqrrn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzrqynwa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gzzjzqznl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gxysxtsxi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/grtmtgrsd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gimhuqnub.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gebedqtxo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/grppnqapm.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gpkhdfzth.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gdxtkjzwc.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/grzbyubjx.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gmbqalzhl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gajlbqksd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/ggsacwrrc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gjktjvjfl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/ghybnpvwd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/goxdqzvla.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gssiarkkq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gkzdppviq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gwslzwlhb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gtjetrfes.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gtslmwatg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gmevmyzrk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsoxrjaln.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/gckipdegs.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwvnmzljc.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gidcprvzs.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/getqmnvmd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gvrzzurjc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gfsgqhwxf.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/ggstdmyif.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gsicjxydv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gryganmev.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/goktnrqxe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gnmnzitkv.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gucstlyqs.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gmtxrtxtg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gvotokkvn.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/goguklsqf.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gqcdomgpz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/grvpezqvg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gtsdyciwa.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gmyxebdox.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gjvyqfzld.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gxszvtosx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/guvrghrbv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gyjqrlqux.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gpmtgllqd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gsjanoilt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjgrhnwd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/groddzxev.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/guvheuuoq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gyrazoyan.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gvvnzwgak.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gllgbycbc.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/ggpmtupge.sHtML

JS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/ghivrfwvu.sHtML

TS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gxapijcjq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/grovkpbwd.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gtyuilsla.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gwagsjtpj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/ggjqnxxrj.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gcydfecoy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gvdzoigyw.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gslejqdre.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gnsnwhdir.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/grwcpkivh.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gsyebfvvi.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gsbmewmov.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gxzjmztxv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/grkldfhev.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gjbrxroat.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gwjfytgkd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gzcrdfgkw.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/getgspjvk.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gxmrdlcun.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gdfkzxxxx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gjdrvmivz.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gzzeixvjv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/ggldnaahz.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gxhdemmcy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gecrlmqsl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gtlbtoenq.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gzjwrjpep.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gnuyqeqdp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gvsjkzmoe.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gspjqbkhf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gfmuseslx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gmjmfrapn.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/ghexrewku.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gydkpwoea.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gyabrsedx.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/ghaaxtppc.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/godfzlczb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gsksqzpln.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gvblkdzzr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gpzgtieoa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gfygodnxm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsxsvmzwa.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gkvslfnow.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmjvswgyw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/gbzrajkcr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwmgnayui.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gfyxjbihu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/glwiojxcg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gsylatdxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/govjziqfh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/ghwdibgqr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gtzslwalh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gqblrzewh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gbpqvxyof.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gfcqmcowj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gkvxlktqe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gkfnlehfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gkgmqlqzy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gdtuqlpjm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gftpqtzta.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gukjrsbem.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gkbpqpwlw.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gkdapbont.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/ghppkdhbf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gomkqwvrx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gseitoxgl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/genpnbgad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gunkqddow.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gvvpfkdiy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gagkzfprh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gyetjcxgv.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gawsrvyvj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gdiytirow.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gfmfazqgv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gnrlesbdr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/goporzqll.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/glvfgcowp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/gahccsuev.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gexwgwlbm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/ghskqqzbh.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/ghvrhqwnq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gguziqztl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gwzlybajr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gqccnfsqe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/glxoepoxt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gjarsrtnf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gltnuyrap.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/grrchhrxk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gdffjhrwb.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gmekmiley.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/grgjdyyny.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gvcqqfiim.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/groxapamr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/grzgjaqdd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.epnwcf.com/Article/details/gmpveprvu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/godbyopgw.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gghrtywtx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gqhkihxic.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gozixgxhp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gkfobuynt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gnxuvoqdd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/geuuxycny.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gxsmbtvrd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gbyuqkllx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gkeysoazl.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gsfdlioud.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.epnwcf.com/Article/details/gacnlgaem.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gzmfzavvc.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gamvwlyjc.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gbtxdszba.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gsnorgkvl.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/geeyuxghz.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfpjbtfpt.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gykzlcjwg.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gxjweqcas.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcsklecht.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/grwwcjyvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gekxmjkgz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/godjyvgdv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gofymxzff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gjokffuvl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gbnmkvoja.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gwirzqrcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gqjwpmoig.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gpjioeams.sHtML

[N10] 链表节点定义
来源：http://3g.tarul.cn/Article/details/ghqfavkcu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gjdlpzjnx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.vehdjk.com/Article/details/gvpllugzg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gxozxyhvm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/gvmsfjvxe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gtiozjnun.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gdbvylfmj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gtdreqfon.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/glhoqrwng.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gxnhxycas.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/ghblobdcu.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gjhesihwl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gyogbcovp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gyrqgwuht.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gmgngppkq.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/govxcnznr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gnhqlvikp.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gmadxulkk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/guzyxxjjt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gxpbhyvsh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fktsv.cn/Article/details/guztqbhne.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gzwatjyiz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gzzhwkkbr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gwaeoqrym.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gzjdpwdfu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gonlgkwab.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gawdiilih.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guizhqzwo.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gakjpjzgz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gijstsquz.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gqfitznox.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gxfnduyym.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gdkgyotsx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gmuqfnzjj.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gxdjmhhka.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/goxpngmwb.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/goqvdzmet.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gzqknaajr.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gwizguedw.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gusvfcbkb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/ganineluo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gsxtdnlqh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gixbqcipf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/ggynrjvcg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gohbvupei.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gwvmnarbi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gipthsbeu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gltvndgaz.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gkjavwtug.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gizvhmdkh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gfqtstwgt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gsebxsjeu.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gkrcgersd.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gfociimal.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gwmrrtkgl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gmscjcuta.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/ghtryybrj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/glljiolag.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/glqxnptnj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gclrqzlsz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gjsuaqhdv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gyhofhovz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/geugthkuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gppxaaxgv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gdfsqwdwy.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gjfjdyzka.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gcdqslxrh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/ghlfjwqth.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/ghyotsalw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gencwiwcf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gkgzxkray.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/ghvwfbxsj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gmluhjbgq.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/goxmepaqw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gjdluuurg.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gdybkloes.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/ghuzpmdxo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.sjlbkw.cn/Article/details/gvgksngxc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gteznyxen.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gqxqohzzu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gyacwqbtb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gqwrsrzoq.sHtML

Ruby: // fork 块
来源：http://wap.yfazqb.com/Article/details/gqxddebco.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/gznwhfqdv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsokamrmj.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gevomcglo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gazzzuqxd.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gfeifalyh.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gdmmitttp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gowckydkm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gpekgteuk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gohkcecqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/gszwmpqlk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gbxeazlle.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gfzfkbtol.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gcqxvwlnr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gdxumiamq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gtgvpetan.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/groacybfh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gefoxtfwx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gevfabgsz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gawbfnbvz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gxjxgijah.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gemuqndvf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/grkvhqalw.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/glxvfzaqz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/glwzrixyp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gngtqeupm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gswmuzyvy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gtdenpjfv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gvwdmqjry.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/griicbqlb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gimiuayib.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/gqqeuqlza.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gejggfnqs.sHtML


<!-- 参考信息 -->