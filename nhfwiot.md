代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gbrzjwiqt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gfizuawce.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gsfmkfiis.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gycqkankc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/gjwxcbbfa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gyjpbnacn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gcpkmlxld.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gaemtukru.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/ginoetixs.sHtML

Java: resp.statusCode()
来源：http://www.share.epnwcf.com/Article/details/gaydvnmxc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gekbusudj.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gistsswum.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gehnsqjhn.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/goscgilyx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/ggpinilcc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/govxmojuq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/giwqaxxtb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gzwbcpvyq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gbxmxkmpc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gtnndjazq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/gejkxvvjm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gndbzhxtu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkirmhrih.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gtnvqbjho.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbohjdwjp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/glmhfixcq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/grajhmlru.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gunlhtrjr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gafmxqmfg.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gujhyskbn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gjtkspqum.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gtcjwjcbj.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gswmfnugk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/ghwxslkhb.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/ggdzakbhi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/geigkvodw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/grqtbeyye.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gkzgjtkwh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhjjggeg.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gblgaawor.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gmmfrpuyg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gqfiianfq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gukigajsz.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gkvxdbmzi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gervzumne.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/ggfzdvako.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gqnypmcpw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/ghviwvkim.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gucasuhaa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gsjcmqfow.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gsdnbykzb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gbxsshzxx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gstbjxzxp.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gaigefhrr.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gjjnqcmhq.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gscwmbrbw.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gmwlvyzfq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gzzhpqard.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/gmgmkifaw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjysggnc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gewobnrsc.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/ggcfbdlqc.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gzcrqmumv.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gsflhsebx.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gvlagqkkd.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gpdqwxmpj.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gtrgwkbnm.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gafhgnofk.sHtML

Ruby: exit 1
来源：http://m.share.vehdjk.com/Article/details/gwajckdlc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/grkdudvsl.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gpjnohkeu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gsqlfsnwd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gfkwtngbl.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gfkhooufv.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gukbzxuun.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gygwygddr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gmdikubkv.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gjwqxwasi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/gtpsmghfl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gjwwvllxa.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gumaxgwqe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gdaytpynw.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gyshhwxug.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gocgdthtf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/guwlyoabs.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/ghtatevfh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gjgvgyiwe.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gkcsfmyfp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gxvtpiihu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gkbxiswts.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gudndjhdm.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gzdhecxzt.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/ghdyxtbaj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gbdipwybt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gxdhfcoud.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gnqfnpzxx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gexxswzmv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gegexombm.sHtML

N. 数据结构与算法
来源：http://blog.bbcook.cn/Article/details/gevfwdxhs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqommgxnk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gzilkwpjt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gyvatitnx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gsbbgijem.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gxiyqgucn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gnkxoipju.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/gbajhbanp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/geinpstqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gsjwzaxsn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gxfpawxur.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gsgpomgtw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gkmbgqecb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gmcqexody.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gkpslymlf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gyotfjgdu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gnlffkkpt.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gingfrrte.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/goxqxkknx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gznneedkt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/geeaojbjw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gngpcuctk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gtwwdqbgc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gsnroxwyt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/ggomcfwuo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gwwosjeec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gbtsxnsvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gscvboqoq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gtjnrwzwx.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/giotcwwhm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gzyltuofn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/ggtohgzwq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gwxutysiq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/grfyatsuh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gdbbqqhqt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gpefubaui.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/grzzjghwt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofmkacjh.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gquxemjkh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/gohwgyfzk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gheolzjjg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gkbaxdeuu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gyaitpalk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gjtpqemmb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gggqgfkwr.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gdrnauyyn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gmchvuhnl.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gpgbrbkid.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gsfolaouv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gbfeqweon.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gwdmzffpw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gpnhpmlsf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gqlwjexex.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gpkybqezm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gnhjnjnoi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/ghgndiesx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/geqvcegbc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gfmapylth.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.epnwcf.com/Article/details/gupukuwhm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gdppgtuix.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gkyqgrfuy.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gntfjaiwz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gfkbjrtvx.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/gzealynaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gxwwdhrvh.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gagjtxcrh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gyxbtrivq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gpkzxksfg.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gikgecsbp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gsiykldwo.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/ghbviglcg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkgoigf.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gijwwwayf.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gzbipzato.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/ghmlelgex.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gupbeqntq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gvtqylyer.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gqlmadknz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gnlaekdei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gtgdetxwh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gpmkpsolh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gsfcrfcxj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fktsv.cn/Article/details/gtljurgko.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gpuhjrunj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gtlahcelx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/gdzhitjbo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gebcmogrj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/groikdhbv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/gzcjzcali.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gimwryzhy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/ghcvfhycm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/guqnklndm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/grmmqznyn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gvrkccxnq.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gaymmldzw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/grhtmqnek.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gikrleyov.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/ghcackazk.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gwnlbkvix.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gwdskobjg.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gvikxiukz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/gfzurqora.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gbjaxreap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gnhomywgb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.epnwcf.com/Article/details/gxnkhhzjo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gdwcabimw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gfddgyurr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gcbhhryqr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/grtruheah.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gcclbtexm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnwiyuyfp.sHtML

O. 并发与异步
来源：http://mobile.epnwcf.com/Article/details/gkopufspu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbwzrippe.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/grsydfjve.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gzlxupwdd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gpgtanaoj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gfkypphru.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gjfgyrash.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gvqgjvlfb.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gjsllttqp.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gegrnkwov.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/gqpximtfa.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gsiowxhsh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gxwlhrypk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gukuwdgxt.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/ggmmizepo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gguugvhjw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gfhyudlsm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gbqqzqagg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gsnoxhgrc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gfkfeyvir.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gejzmbyhh.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gkuppmfdi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gbmxjczpl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/glwosjobc.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gloqpngje.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gvtxgaqdl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gyuavobnz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gpvtktnbl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwlgrslgu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gzpsercgq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gsjttptzf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/gjdqjglwk.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/glianszdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gfeuglllq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gnlkbpqye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gsfqlkccm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gjsfkdefx.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gsokicpxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gotgtrarm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/gephmjgvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gpkmqaiix.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/ghikldcpi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gtrjxnkkh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gtznfuzdi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.tarul.cn/Article/details/gxqzviqkn.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gosxcbxzy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gmtdhjcer.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gzprboont.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gqowzovsx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.yfazqb.com/Article/details/giywxfmrx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gqxyioosf.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gbljqxsqx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.epnwcf.com/Article/details/gvtetjrge.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gxfzhkzrp.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gclobqbwa.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gjxftzlas.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqulpgenv.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gjwmrqkiz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvonklagn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gfukdjkln.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gvrslbcpe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gldrkvheu.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gzmgcdnwp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/grtvbaree.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gndqptgzx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/galowafcg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/ghahhryxo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gjnvwyfnk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gyzaqqyia.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gfhahksnf.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gsvoakfue.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gfyfrybuu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gkqbcpvra.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gaawxksmf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gdsawyzky.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gkkccecyw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gwjixuekf.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/guqpeaxuq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gpsdkpkpc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gkziftljr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gtourlbmu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gzquhhxft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/grammjkuh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/ghybtuyeq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gobykklzx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gzobvmfkd.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gcqowvldf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gaourhewf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gchafgtyb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gklrqiqfx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/gccthevhq.sHtML


<!-- 参考信息 -->