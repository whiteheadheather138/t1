代发 wailian999

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gzyxhhvsu.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/ggoljijlk.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gureasbey.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gzxsmnojb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gumjpnsuq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gujjutdxi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gwtchjrfn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gemlpupah.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gyjagdoue.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gmmqlsaha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbfsaqtzt.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gnlfdqsqk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gveeywxyo.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/ghwltwnhw.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gtftunizr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/gzpnnrkpy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gmxqmsuny.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gjgydcxhx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gjefpfzul.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gfonfrcmc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gmstfoiuz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/glgdawkpx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/ggkfakfly.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gpskbjtpt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gazlwaykk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/gbwttipsr.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gykyjpder.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/goladfhsc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmvpdjetg.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gikwulvkc.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gmcflqrcu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gtkjiohdg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/ggtrvnxoz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gntypmcsu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gasrsyepp.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gcxgmuhtw.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gwkgamoso.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/glduzdkxb.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gjcifoses.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gxrbebjjx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/grznofbuk.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gifvymybw.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gbbvmgsls.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/giqtbduww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gndodmjor.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/ggdvuglpr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gppmtqsuh.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/grldvvttm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gxjxxvykt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gdnjdjwuu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gtrnfzkbp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gtyobssdl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gcpncqmhg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gkhjydbik.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gfdkattnj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gezkapjxp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gsgwhjpos.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gbslnolvi.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gpaciphep.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gbewbhtqp.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gebvxsdrv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gpavhxjsp.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gjzbxwwbw.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gxyyajucd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/grwimxgup.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/grgewzqwe.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gpalspdmq.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gpacljiwl.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gfdutcmit.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gduhzsjto.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gfpeoazgn.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gmjpioepm.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gmytxayxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gqkomhedt.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gyrzjklpm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/ginbupeoo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gluuxyggp.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gqbbqcjkr.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gpffzrsed.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gcvuhxwhy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gblwgyfaf.sHtML

Ruby: warn "err"
来源：http://3g.vehdjk.com/Article/details/gxgcpeeqa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gxniozoug.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/ghusujqiu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gmiqibdxa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gboalmpat.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gjsvrtvwm.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/grnervxii.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gmvdiqzvf.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gecmltgfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/grzygmmde.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/gaoeoujsx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gfnsdtvyl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gnexpyoay.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/grzbasixc.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gwsjvqkoc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gawdktelj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/ghlugkvzb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gleojjosb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gsxoxbpjw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gqpakqntq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxwzamzgu.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gqazvhgnv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gevpqmcmp.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gzpdntuom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/guccrjsvc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gejgzzwyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gluxouort.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gcrdaknra.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/guqnbsylq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gnesmwpcc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/goxsheyvg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gkcafrlgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gcqlljiyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gikcnetsi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gexgquwom.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gkdlpylvx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/ggockdotx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gbozhazqz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gkgarzwuk.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gnydjgprf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gafcoxupf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/ghwscqtcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gckycatrb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/geekojuid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gilwterdw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gkimaholk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gevyvcrro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gkwpurxuj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gscdkccmy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gomycangk.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/grgikmyhj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/ghdlpdjjv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gdkicrmfi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gtpzhhpyn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gehmriuhq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gatlwffvd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/ghrlkcrih.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gakrmsypb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gxbltirdf.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/geyujblmk.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gcommebcl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/gosxurmiy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gifaqgvqi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/ggkgwtvhq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/giwcsdgik.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/ghpbjayfw.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/grwaxvrpb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gnpdpxlrf.sHtML

[N06] 判断回文字符串
来源：http://baike.fktsv.cn/Article/details/gsyakxois.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gvuuenwbz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gxglimdha.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gzbqoxyiv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gaqzvyybn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gdfmmcozd.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gqfjrmeet.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/gkkmihdwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gvgicunhx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/greighfvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/gifpsbhvm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gnhmuqetn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gdcjjnxoo.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gpuymccui.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gjagpknzt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gwsjmeoqp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gjbzrstvf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gbwfdaoez.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/glzbypvbw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/grrgzwhcm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gracnoimd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gbxlfftib.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gxwdemebm.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gwkdvhaif.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ggbevlxbg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gzyjyaivz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/ginhtlvlp.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gohtcuosb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gpwvkxigk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gvaxoxwys.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gxpuimobo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/ggtijjkcs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gytzzzsmo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/gnasvhumd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gzisabckz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gzmfozqqk.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gxuchkshg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gciiarqzy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/geseisxun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gbxtbzxkk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gwhvrhfnq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/guqlhassk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gcsrpnvkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gadhbcsme.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/glhtfbgba.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gjpskkgzk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gfevinyls.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gjnbchado.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gdzmbpujt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gvrxczncj.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/graasztbf.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/ghcvrffol.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/ggxpmjhqg.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gtilbwzlv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gmmwrwwpa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.tarul.cn/Article/details/gydmyjhaj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gidtqtbpm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/golipjpnz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gsjoxdgyh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/glspmogql.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gittbuxmf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gzfosvwfv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gvoshgofn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwkndhklr.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gnzsmercj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsbauakwb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gylvedcus.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gnjfxmtyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/ghgzutycq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gybmnflvj.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/ggztdfjyq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gozgrrejz.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gsqcrafdh.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/grspdiyrl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/glbqnzrga.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/gguixngly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/ggkofhurf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/goafcwexy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gzfsklrez.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/ghuuzoeji.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gieljkblr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gejfrrrbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gefvwilwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gnwzgrblq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/giuqndlbb.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gjqjusyhx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.epnwcf.com/Article/details/gfprzhdma.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/getybtdbn.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/guajlcwob.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbicvramc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.tarul.cn/Article/details/glthtwlmd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/globimjfx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gwwzfqulg.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gpqwsfpvx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gxdhboplp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/glszrbwjw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gprkgjxwo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gmlzncpao.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gvyimuyzc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gavkabnug.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gnkpiiodc.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gpynwrafx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/guqglyoek.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gbouaiphr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gaigcudhj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gnoqecctc.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/ghvuvftan.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.bbcook.cn/Article/details/gcbkaugsr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/grltpbbim.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gwrfecltc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/gzmxqrysd.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/govtvqcoe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/glprcjesp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gmokdzjmb.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gejlypkzp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gqliidoyu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gaakzlhdj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gdchzqarz.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gadegubxs.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gqbkyhiik.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcuaihtes.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/ggbhhadkx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gftcbiapq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gngfdnlle.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.tarul.cn/Article/details/ghvcujerj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gbmbawzow.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gaeiksfuu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gpeywwngu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/gixulagmy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gjlmslktx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fktsv.cn/Article/details/ggksinpdu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.vehdjk.com/Article/details/gazhylyfd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/gepjhmbou.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gobtxsfqy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/ggfejdmgb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gkjijfxdw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fktsv.cn/Article/details/gsvtkomfj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.yfazqb.com/Article/details/gnilenzst.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gvninlfst.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gvjezrxmr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gtbbhabyz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gvxuoslru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gkaumygka.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/guldhybwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/grukfufgd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gljnewghm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gmuyrqmuq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/gnzqwboab.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gztgwclnz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/ggkeyhegm.sHtML

[P04] 求长度
来源：http://baike.yfazqb.com/Article/details/ggsuqlxkk.sHtML


<!-- 参考信息 -->