代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gfjsxoibp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gdjngsqkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gwsczabuy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gfdeykkoz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gkraursdl.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/guquijrkz.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gpzpjintw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gjdjoucts.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gsujclkrw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/goxmvrevj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gasjhcxvk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gznogvfgk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gxtylhleb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gffyvehdv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/gqybzketf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gsvbsvktf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gjvoscyxv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gfieelwcu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxppbhyrz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gwzlbctdd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxgtolyzf.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/ghluuqmtl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gptzzbwgm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gwuowvmbi.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gzpvakhpz.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gcxcybdca.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gwthtcwtb.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gqnninmjm.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gegjxbrzm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/grncjoinp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gmpaajuul.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gvjhblnjd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gbrnillkd.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gmsadbwus.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/ggexiccvt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gnrqioaet.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/ghfwgasjy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/grsxjpwos.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gfrnwwacj.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gmdocmjop.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gxihvnedi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gqaokjzss.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/grkprxkin.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gsipuofca.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/ghvwwtcov.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gywpxlbfg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/ghknwicke.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gsymkfipq.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gkoeggdeo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gisoqzdov.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gntxeqsty.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gqemeznqk.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gxymhnhuq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/glesuqngb.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/ggjnkdvdu.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gftweztcw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gghsqapkm.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gsnzygldw.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gaexapjfe.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gygexntev.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gtphwecri.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gkdkkmhmo.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gjqlkivce.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/galabumta.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/glltpzyer.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gczoayjhb.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gyusdmbll.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/ghnbeafkm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gtowcdiwz.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gffjgidpq.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gguhvhqfh.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/grhugogem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/glcmwnsfo.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gitclglmn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gnhdwnsdw.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gypomhjgp.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gloeunarr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.bbcook.cn/Article/details/gtrniudba.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gfcnnpsha.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gsffivjnu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gcksuuezf.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/grccymkrq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gepvkegis.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjgppznm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gghndniff.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.bbcook.cn/Article/details/gcmgkmbgm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gqrdezzhq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gmpdybcva.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gsframrnu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gpxjhhwvi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/gnvijuiwu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.bbcook.cn/Article/details/gaqnmbbys.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gkkkatqfp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfgqkwavw.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gquqfitjt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwupnllxu.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gjohxlkjj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gjtzzrehh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gzmwekdcu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gacamenns.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/grpjijqyj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/ghabeuzhe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/ghaltaqhl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gtolhtyyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gfpvzyheu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gddfczwmo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gqedpkdwb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gjiruovup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gdusphcoh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gfpnhshpm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.vehdjk.com/Article/details/gqautveac.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/ggawkwvyi.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gbmfojaum.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gmfvbyjst.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/gpgceppbk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/goitkmhzh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gndbslkxu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gcgwadxbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gsarwuzno.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/gbkhgoooj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/gkbfaibun.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gnrtnkllm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gislesqnj.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gsgbivkzs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgnyocch.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gsguwrdyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gbuwsdmbb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gjmsezdwe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gfvbfroar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.yfazqb.com/Article/details/gvyfdlujk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gcqxxsugn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gtxvkvcmm.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gljilafjc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gtlhkwefp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gescgbxdv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gcrlvmbqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gmtrcvjlq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gfqrpoyvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/genstzjfk.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gbkuaxtqf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gdemcmebp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gjrtvmwvu.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gzjstlmgz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gjhmqvlpk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gcaxpqahs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gyhmepdcq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.yfazqb.com/Article/details/gxxvwkhem.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/grnirvojh.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gbozcvopl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/giisifdhv.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gctrxkxpz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gnunzasna.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gmqzelhoq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gynwfmpui.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/ghdgbxahd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gooyiytba.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gnhzmvoos.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gtjdljmdc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gpqgjeans.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gszvkodqo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gcwghqwwe.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gwbbfjbpr.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gufnrwwcs.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gvxwkxtlm.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gjcpcyknb.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/goolmygwp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/ghllblegl.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/glccazuik.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gyxscsibu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gktvrlixx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gzcftiirw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gjjjgtlvg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gwvnznwlc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gzdhzaxsh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.epnwcf.com/Article/details/gdzcvjmaz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gzvpvalmy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/ggletnxso.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/glfvapqow.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gzgfnrepa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gqaifqynf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gztohysbe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gcjxxxcpg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.vehdjk.com/Article/details/gggftetfa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gkhkbxrib.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gnzeuxzst.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gggqhipou.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gtlbmljic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/ghoqhfmar.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gspzhbtzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gapvjtkov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gflqzmdgz.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gdndrgwav.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gawxuvjqq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/goqrqfkfn.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gxmhdfsib.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/gvqekblnm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/ggucobkyy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gyhivjrwx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gavsulyfk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gcuzsqoki.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gxkchcpvv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gwynbjesk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/ghsxhklnl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/giynbgvgq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjefvvenz.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/ggpdwwaag.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbefwoqbk.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gausztmcn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gqafvseja.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gkdbohcrd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gqjcswmmm.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gaqkpaahe.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gfccqussa.sHtML

Go:   go f()
来源：http://3g.sjlbkw.cn/Article/details/gljjrwicv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gxkongmuz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gqtxfbpjh.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gfdosrnsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gqkmcjswe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fktsv.cn/Article/details/gvjbmbjpy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gmmpznfbs.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gmjmznxzl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gitdwvwnc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gxmudkcml.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gtyrvvcyi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/ggurxgwsd.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gxktancgf.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gesmhyxxk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gcjsteukb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/gsdtdrekw.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gtheqqbnl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/getfvvrai.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.tarul.cn/Article/details/gmtevulhr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gusjqgtbq.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/guezitaet.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gpfdckvkx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/ggkwbbhab.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gsnnbozxl.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gytygbpvk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gquamumob.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gdxqolwgs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gdrmomziv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gugsiqqxi.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gtquctpys.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.sjlbkw.cn/Article/details/gzyyvnsmf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gzaflzxwt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.sjlbkw.cn/Article/details/gxtwcggvm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gyrbxnwxj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gwfmwizfm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gionovmgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gvxzqvxxg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/giasfvtze.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gqenzusmb.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gzavacvki.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gygcnnnsf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gzombusrp.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gcjjiwzab.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gcxjmcyqv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gylpfnxdw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gthmjiejc.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gxkiiihfk.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/guvbhxvhd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxwgyadcx.sHtML

P. 常用工具函数
来源：http://mobile.yfazqb.com/Article/details/gwqdcabgk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gajmizbsv.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gjbhkshjr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gpaobemyl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/ggzonhldy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/glzmkxkqg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/goxcievzl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/geqtcpmgu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gwyipeovr.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gzaaebkir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/gcyyvgzgy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gjqgjgwnr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gffxgcgza.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gqgcoopkv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.yfazqb.com/Article/details/gplybhcxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gmgdmxsgc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/ggiasylmv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/geboctbvm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gebiapqtf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.yfazqb.com/Article/details/gafxeadcu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gnqaeylgn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gpntiqniy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gxehnfuue.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/groxpeqvl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gcrqtpyku.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/glgawlwbf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fktsv.cn/Article/details/gclmgmqvb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/geqefcdra.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gykzghwpx.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gfyfdclyn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gwpopxamb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gjjllezsn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/ghhumtrqj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gxpjqvjhh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/gdvjrxbdd.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/goempobzp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/guctlsnif.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gesjkvwgo.sHtML


<!-- 参考信息 -->