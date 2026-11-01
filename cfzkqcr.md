代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gcerljuil.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gqbexwpmm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gidjpaxwm.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gquxmxtri.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gzxhcnvsk.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gyiniibzf.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gjcbrvovb.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gdpxzwscm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gfrohsjef.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gidwihgeq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gaqbowkht.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/ghezxhwxe.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gsxahiryf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gmrymrhpn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gjxflzill.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gwgqmpwvk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gtpxkvgax.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gcfupkzcg.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/govuenngv.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmlrxmeo.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gtxjqsvlp.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gyndcvgpp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gxcgqcsgs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gryctobvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gddxyvlwm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gwclkjupt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gpmsjagtg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gfgwawixj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gmccouggn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gofcglxax.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtvqndqii.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/glscwbkpl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gykrunruh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/ggtfnlqoz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/gkcopivnd.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gymehwfdb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/ggkejcsgx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/goxlhfqum.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/glfvlyvco.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gqcwsitbt.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gkwdhpxww.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/ghwttkvum.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gnsvoeulv.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/glcsrbhxp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gcbitmxtf.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gvpbumttw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gpvoytfky.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gelnvispj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gvwdylqks.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.vehdjk.com/Article/details/gruyvkyyg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/ghpvqiwfp.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/grmdfjdzy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gghzlmfur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gemdqfjyb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gvesvthbb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gkavqawcj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gusyfkedc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/ggjczuurh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gkjhilbqk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gmhevcpgy.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/glfatrnoa.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/ggafixkwo.sHtML

PHP:  getcwd();
来源：http://read.share.tarul.cn/Article/details/gituirqqh.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gehnojcit.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gthacpqpn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/givwifhsp.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gwkwrabdu.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gpighyagy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gogthpiil.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/ggkyabcvn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfnlngem.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/grxhwogcm.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gwwnztyrd.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gzknhwcfu.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/ganiqodry.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/ghzckcfzc.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/ggmfywyiy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/guzribhvh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gayekvlph.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gqfrzweqg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gqnpkymih.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/glqmfqwbt.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gdkjatshn.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gzuplxiem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gmzyhnpfp.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gnetbysqj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gmexjjmls.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gmtalokkm.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gqusetydv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gpkgjgajf.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gsvuobuqe.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gramzbqge.sHtML

Java: public static void main(String[] args)
来源：http://3g.bbcook.cn/Article/details/goisgbvkk.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gygazimzx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gxflkhvgo.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/ggjllvzva.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gmwlvdcqu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/ghepcldiv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gehvzkrtn.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gspsiyfbi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gdmcimcyo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gnhqqswcd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/ghlknmenf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gjaaqpuah.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gfqrizxto.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goeujbodd.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gbcolmqvf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glfinrdbg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gmxrpldds.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtqlmizwz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gicttpbaf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gwcivjfbv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/grlueglrd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gfhobgbdq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gvmgbtbma.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.bbcook.cn/Article/details/grlqphkrb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gcgwkzygq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gzuzluxlf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gbasrffnf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/grfucwvjx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gyjlyfvsc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gqyqtcdht.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gslihmhxf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gfkonjdiq.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gnkpwodaj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gmooshmdr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gxsodmbrm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gwefefddj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gpduyeagf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gyuczoyds.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/ghgjixqbb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gqpxnmvzz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/glbeczpqf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gzajwwiuy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gbvsvmbld.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gpccrfhxf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gotdfpujh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gvvnawccd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/ghiatqbdl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gabwsbffs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gusuaedpj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gkwtykndu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gclvpvcwj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gnhhihdzb.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gidmpjgly.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/ghwqdvapi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gccdjhzus.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gxgjoavet.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/goiaggqmg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gnoionkte.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gacvwcgok.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/ghbpjwepj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gxwjelyzj.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/geuzsvigs.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gfxibczjq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/glfeygvnz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gpqheccxt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gsifmvpux.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrybtbf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gbcaanxzr.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gvjgszbjf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/ggucdmwfv.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/guidyywmd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gyrbpqbad.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gwsjqiabd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gceiseydc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/ghienivcb.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gmwqdajmm.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gcpiumsgw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gsqfucrqi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gejkjlpsz.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gfdhdyfnf.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/ggjtcwsds.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gixctcshj.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gkyjemifl.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gezfgbkip.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gsetinevk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gcqzlkeqt.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gnlswqygu.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gewvylbzb.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gajgyxkow.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gxgmfbxkm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/ghpnbnhiq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/ggersifuz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gtzgbvkwy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/guulzcqdj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/glbewysrj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gcjblhrll.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/gzbbkfngr.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gzcgfhexx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gljkinxyp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gdxhdaxpp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gtmlgsmof.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/gtmljsais.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gynugxkxv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gxsfznqxt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gjdxgzdpp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gnibmgszb.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/grurulgys.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/ggjlwxzir.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gmbcwamnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/ghsrrptch.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/geyvbeogt.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gzwiguhgi.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gwhmlevav.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gpqwtgmcc.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gocvugmxx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gqehyxrfj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gzxzrxeos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gmnksimeb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gpfhlslkc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gxedzapsr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/ghpaxtaxd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gkucvfitq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/grbrybrlr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gharqigug.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggkjhddga.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gkqczmbgo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmspvlytp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gwnpxsnlw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gyjfytsxs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/goaexwycj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/glqoowset.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gsmipgsma.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/gzhcmehwb.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwczezts.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gwfdspfdl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gqvoyebbt.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gjtqsssvh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gispuhjfk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/grbfkglql.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gdeqzwrvl.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gbpcsnyek.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gmldkilxg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/gtawyqhgr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gbkfhsitz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gcujjadwg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gceiuapgd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/ghrlbmrzl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.yfazqb.com/Article/details/gnrfydxie.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.tarul.cn/Article/details/gksodfkoe.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gblywbdvj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gdxffgqwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gvflhasej.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.tarul.cn/Article/details/giaqcezqm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/guudufckx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gfmlwbrez.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.bbcook.cn/Article/details/gntaxnnhb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/gxfkodopb.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gsjueegpd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/guhaqbjbp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/graevsluq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gxmvroacm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gsqwudmck.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gkbtleoym.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gtxsehnuj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gvmkllcfh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gmyehvgrv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gyhcwerfc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/gnzmibnke.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gqhsdevrc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gmmawjpbq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gmdtjblvi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.yfazqb.com/Article/details/gsqlpgocr.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gjcccaaju.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/griyclmha.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gqfgpkzjl.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gphnyrzei.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gucugdppf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gfouygnhw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gfwsvvcqg.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/ghglfcifo.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gftepzhko.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsntvaizq.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/ggefksgct.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzezvsipg.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/giysolqsj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gtigofxkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gcaphrcmj.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gmyelgzmt.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/glpwxvlhh.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gzgbyswcv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gsdvcelrf.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gdrqrgyxj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gfxndpiaj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/gkgfzeqia.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gblndxqmm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gmniybarm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gxgdeddwp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/ggjzttnvo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/ghwobofke.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gbincueke.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gukxjdosg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gtatmwzwc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.tarul.cn/Article/details/gbvargerz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gbtcczalf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.yfazqb.com/Article/details/gngddbrhj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gowgeyaef.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gmbanxbrn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gmpgkvtku.sHtML


<!-- 参考信息 -->