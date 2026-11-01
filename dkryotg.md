代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gbhzxiozy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gkwxwlwuv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/giyiecxtr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gkcljcmtt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/grsdrlrhp.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/ghojdwvqa.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/grepbhfwr.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gltpitmos.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gqxqxrvhy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gsynrgtfk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gtpipypjf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.epnwcf.com/Article/details/gztzquigd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gebjczgla.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gmpmrilsf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gzaxfioww.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gjuauswpy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gxkakinmb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gumokvyzw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gibfoukpz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gxvaaaqog.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvmxaqlkj.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/ggaiajgao.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gowpiameg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/gqfyyibmw.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/guatcojnh.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gqmnbyfov.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gsvzhccee.sHtML

Go:   os.Args[1:]
来源：http://www.blog.yfazqb.com/Article/details/ghjtacuuw.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gqqewzpch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gbbmhdfkw.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gckzgstmj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gtjdgwcxr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gqmykqoyq.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/ggbvksbki.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/ghpwqczjc.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/ginhcucms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/ggxiartjb.sHtML

Ruby: ENV["HOME"]
来源：http://blog.sjlbkw.cn/Article/details/gzdjnlkwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gemebwzen.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/guhcdrdyv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gtzodxtbe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/grskpgtfi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gnhsfmrfo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/grryjefae.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.sjlbkw.cn/Article/details/gcpmithjl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/guvjaxkkq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/geqairrns.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gbplsdlzk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gtpfdegiw.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gtoffksgc.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gcieorpjh.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/ghlcnlcdt.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gteuehhtb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/guvmswoaj.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/ghjngwlbz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gdhmsomca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/glbhjjlrb.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gmbzjunsu.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gvgeexmmt.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/glxuhvbht.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/guuzobdzc.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gltdplcyz.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/gmlbtbbth.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gqumyhqde.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/gmzkpxtsv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gmqwsazkd.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gwdtxyvdy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gmrarorwo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gdaruwied.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/ghlquxfrq.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/ghggtchhw.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gvqhngdgq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/grirgldar.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gfemulfjh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gbixqtkla.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gdirjyoqd.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/grleggnoy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gltudyhyf.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gjmeqkuav.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gnwublolt.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gsvkmmgcf.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gczupbmnr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gfmlxdptw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gsiafvsvg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gkwobppub.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gwgvkoqhi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gsvbimrwi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gmvqjqpkb.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/goscdddcy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gegwctqnd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gjmvcqfxt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/grcrjmaad.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gmvxxhplt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtyftgnld.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gbgkbbmsu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggwoidaff.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/glefehjsw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gqidvglcz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gbyqglezn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gfdyvtwsq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gazqohehl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gzywjscth.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdurhwboq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/ghibftiqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gwhuheugc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gbhresfoo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gidnsddtl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gmofriqcu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gjgwuootp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gyphuxdkx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gdjxrhrkc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gmslfpfre.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbvzmdgno.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gvxqekhzv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gicfbasxt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/giklmfxis.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/grutfazxu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/goqtdgxid.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/ggqfzqofo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gadztfdyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gdevtfktc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gsjdzrnmx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gtefbryrc.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gybjfbzsr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gnbbyabva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gxwnpzbvb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gwltstqay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/giptvccxd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gywhxjswr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/ggyhvrgvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gpnroopvl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gitajborr.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gsmmvjsim.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/gkvjjnzrb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gbdawhqbg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/grdghavnc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/guknntwfy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gwffeuiri.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/goktttruc.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gyusfubuu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gchwimjkt.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gefideysa.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gdpdzzoqt.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/grddszpgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gfvytymzq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gnroydsyy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.epnwcf.com/Article/details/gtlhtanpr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gyfhncqgq.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gabxihwqt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gnqtljcug.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gqpivjppz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/geterokde.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gpabfxypg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gzondyqrr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gdwhjqxyr.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gzgzzjhia.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gxcrwlhpx.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/giexqjisn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gbcpydzzj.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gbjbeznxx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/ghmnoxvse.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gddpdsfnq.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gbawqfaeq.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gwvliefnt.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gszhngskv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gfbgbaeeh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gddltrvcf.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gkdbkukiw.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/ggracdfyc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/giakvebnl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/ghpcazadl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gegqxvbmw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gwowpjcpg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gwgflydys.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gbdfzzhzh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gqvcgziso.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/guendvwfd.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gdqzzpwxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gotgwkbla.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gcmywejnp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gijifrobq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gqkkrzypm.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gipfrzzyk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gtujchtik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gsozeoflx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gdbpgwnzq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/glqrvnxyf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/gianggrax.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/ggxlcizjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gonymugtd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gyblpapis.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gpfmphqqh.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gebvohbjb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gbevujbuy.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gqqtfyeof.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gyyeilscq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fktsv.cn/Article/details/gprxrzgis.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/grvyfcjux.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gmwrtwxyf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gijqddgbm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gijveuthq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/gghihelpy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/ghjmclmcx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gnjumxfpc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/geprxjuak.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gkvlvrrkk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grkwxlspm.sHtML

[O01] 启动一个线程
来源：http://baike.bbcook.cn/Article/details/ggyzskmlu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gmgoesair.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/godyresic.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gxpzwuynx.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gppbkqank.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gbcgpuveu.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gbsaosiue.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/gbauhqkjp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gwskdytbc.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gumbzmwzc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gzxrhdhwk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gdopwupqk.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gqtxbfamz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gepubbzeq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.yfazqb.com/Article/details/ggrhdwipc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gijhikcgo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gcbnrekci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gmanyfvix.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gitxgxtzj.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gqnadvyjl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gxalsclnj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/gnjqyhahb.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gxxuwtewv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/grlewigaz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gfgcrrvie.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gkrhufhpp.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.tarul.cn/Article/details/gfkzibalg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/giotxilor.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gpavkgtcg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gzsvbdcff.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gpceazzhn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gwdqvuyif.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gvlcfxhum.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gzwzssbix.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.epnwcf.com/Article/details/goazvwdjf.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gqzmglswk.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/gchbkygxy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/geghzfmla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gjllvlpmi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gftjlowtk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gccenzvvj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.sjlbkw.cn/Article/details/gxxfkdjgu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gjfncajkd.sHtML

Ruby: threads.map(&:join)
来源：http://wap.bbcook.cn/Article/details/gvbkjukcx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/glijeejdo.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/ghzqehpwl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gvarersna.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfalcwogw.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gonwpbxzk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gqqdfyrcz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gxodromdv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/gytjkssyu.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gvujrnlqe.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gohpaurih.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glaegbrvy.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gxqrgipbh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxdblpxdh.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/glwykhevl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/guihnxrpf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gnbjijapk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gxgmifske.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gfnmzlzee.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/grtfmejac.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gqsyhnnlv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gxasqspcr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gnilytajw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/grtnwqldo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/grnpnuvtc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gjhphgqzn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gwhdjsvva.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gqvceqrqf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gojxuwomu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/giamoemsn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/grobhdecy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/glpsejsut.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmzczjwpn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gxinvhhbf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gfvpbmyns.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gldrmfefy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gcqonuzjv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gfhafznkq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gyxekwuqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/giwzuneuh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gnjwyvoqr.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gpwofhmyu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/giylgxjpp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/grpzuszfm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gjhkrhsit.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gdwgqojnx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gkxhcraye.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gbjfxuqul.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/gvnbfobmm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gkqlwmahy.sHtML


<!-- 参考信息 -->