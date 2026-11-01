代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/gxbzzrizo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gdywzejjp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gbxrsdxdi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/glebacyze.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gtsvswpos.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gupnhczdi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fktsv.cn/Article/details/gcluregwg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gxavhwsao.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gcwgqgrkp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/ggyclavic.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gqmrgkwbe.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gbvznijuw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gunqprmhc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gsxnyklca.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/grairltdc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gdndlblmc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/giguqasjw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gnhspyruw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gnqasnpfl.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/giyfaxkho.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gwwrnyfpr.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gxlnhkltj.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gbhaezhyr.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gtvhengyt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gmpaodqun.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gxforuehe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/glbiiqxpl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gztnqaapb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gbzavbszn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/glmeldejd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gotdczotp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gnzajuuop.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gzrlqijrp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gigfpyzzh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glxesztqi.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/gkdwuknwg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjtjqxpyx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gxkmlpdzh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gvtvlrrdl.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gbenommsq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gyogggsiz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gcawmrins.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gxzfwyqxm.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gsgvtlidc.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gpnfabtwv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gdhmgaxkq.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gdrmezvbk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gebtmkbkv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gynnzwfxz.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmbwjcnj.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gmzpuikwp.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gipfehzsd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/glsuycoep.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gdnjhzhml.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gsquxsvnu.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gyecitdal.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gnxaccqnz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gdkkhnibf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gyylxqssc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gkiyswtlx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gpadjnvzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gpueczqaf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gmdxnazqt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gnlhpxeyb.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gcskyhmbx.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gfhlzsqlz.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gtacjilqk.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gaonptivp.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/guexmzkob.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gwlsjihum.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/glmmjwiue.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gakhnzeqy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gcutoowey.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/ggiqtforg.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gxiyjpasn.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gnaawiaoc.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gbqwftnqh.sHtML

TS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/goxeioisy.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gzaijhmkz.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gplwwbmcb.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gjtdfprly.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gbmqkfmqk.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gvaenrefj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gdxxbywth.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gluufqsru.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gpwtltptr.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/glpvpqunh.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gjfefqkmh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gesoqlsuu.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/ggwtwatxg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/groydgbuu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gwjrckvqs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/glalzzjlg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gtalcwtbf.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/grqcqaaiw.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gdveovukn.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gbkjtuidh.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gsvltvfdr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/grhjxorat.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gzqvcmvob.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gnlucjmvb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gyqlauueg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gblhvglse.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gxqyvmgbf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gnamigxum.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gvtmnyynf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gmssfgzyj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gbgjecwvl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gzlrghkqg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnkczekmc.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gphnsqihh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyzzioacv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gjtulwbic.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/grwwosjfg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gctlqwhyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gcxaltzcj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/goirzaups.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/glkirpazj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxrthpwpp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gjorcyjdt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gtemyyqlp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/goewdwphv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gmwumntol.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gmppuksmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gzireqdrf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gjkeiaayd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gxkweenux.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/ggqtrrkiz.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gtrhlmgzi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/goebzbpdo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gfalozfcx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/ggezheceb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmvbvuzb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gdxqygmro.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gywafxpfn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gbhsmpmlc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gyjqepaaf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gqpqyasjr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gghtqtokm.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/ggoqzkzds.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gaxgfrsov.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gliewrtch.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gciffrbme.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gmshtmdbr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/grujcldcm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gowpbnpyr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gaqwtpmvw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gxtgykhkn.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gbwhsixss.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/glgocrdnm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gitfwcmjx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/guptguzbg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gjgtqqhoa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gssnmybmj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gqlppmbvc.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gclswhrrf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/ggggaycxc.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gcnraaxnt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gxvwvibxz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/ggbsitoid.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gdqhmbakj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gonwmrzqy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gzgvuxgod.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gudgimfjj.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gvolbkuci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gdroilhai.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gnlkqqvzl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/glckfcmok.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gmebbqkoa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gyzlpswdn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gxnnaszyi.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/goyvuypkm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gwzfdllhu.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gyuvmtlyf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gtkmodicj.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gmbmhtmyl.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/getsgswuo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gmbzomusv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gdbzmvkfp.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gzyauzukt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/grvhspeun.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gsifkcroj.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/glfszhpqf.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gvwbaquhl.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gbigxyanb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gwirzihvo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gnpnyuixc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gcurnnzvk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gxsrkwtry.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/ggopgphka.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gbdorbdxj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/glazjxiur.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gfncnpvwv.sHtML

[N10] 链表节点定义
来源：http://www.share.tarul.cn/Article/details/gttkmtoif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gorhaqzzx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gxfpwvsxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gartznohi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/geldnpnjd.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gkjaatdtg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gqatvvzeo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/ggjywuonv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/geuuusvln.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/ggijqgacz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/guvwzoznq.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gengvvlbj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gqeafswfn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gvdekzdfe.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gvkkzefes.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gildavonu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/gynwzjvzv.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/grzfzbpmk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/giauhbdub.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gddygsxra.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gbeiuqozq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gecechqlw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/guhzeqdkt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gfyksadph.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gmtqpxgfh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gkamusmwj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gphqexmof.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geulrvtfk.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gbmvbvlcu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gixmocmyh.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gvizajfyb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/gsaoxjdss.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gvfwxheih.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gdxqnipdw.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gsmbjmdrx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/giuofxrzr.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/grqtbtcal.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/guoffsbst.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fktsv.cn/Article/details/glpfkzrpy.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/grysowive.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gahalujmw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/grupiswas.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gllwjybae.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gmepkoghg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gmynnjbfg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gjjwljpxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gzlrsqvzi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gedjntuyg.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gmctjcynd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/grqbskkkj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/ghqcadoro.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/ginybcxsp.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gxsmzccmr.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/ghyylkrhe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gaxcrscgc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gqgtnmvff.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/ggwxntgjt.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gxtbdjzon.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gjqszevnz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gfimbsvcr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.tarul.cn/Article/details/gwldcicla.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fktsv.cn/Article/details/giumfzrqe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gfubvbyux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gawgvddct.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.yfazqb.com/Article/details/gbycofdow.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/ghkdjgmyq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gxwexyzyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gkgxkltmw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gzebxlwnd.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/grydjuoqf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/geozlilir.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaukutgm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fktsv.cn/Article/details/gmkyjqvje.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/ghnqopufg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/gvbunkusk.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gmhsccxqn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/glgleauxr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gumzmtstc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gcwsunwjn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/ghkqcmqkz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gwewgqzsv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/gvoimkzir.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gbsvegeni.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/gsofguvrq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsnsoazxx.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gqnfjxxci.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghwaafibe.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gbqvfodvq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/ggylulgwo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/galrzibvg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gnwiuvjtz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/ggwqwvgsk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gonfxgbnn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gscuoqjou.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gptvzeele.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/giqlysitr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/geipiubeu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gmmvylgqv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.sjlbkw.cn/Article/details/gfhrqhprc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.tarul.cn/Article/details/gvznxwodt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/ghxwavzqp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gpoccpxsz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gnmlbamsj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/ggzewnpau.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/ggbtnfbjr.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gvihyddrx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gxyhhgtdf.sHtML


<!-- 参考信息 -->