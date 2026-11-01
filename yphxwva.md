代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/gvpwqgjyh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gjkmgrxdz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpirgfwj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gyzajtsux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gxpwsltez.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gwhrfjoau.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gxlhdhpoc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbsuqftl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gmdjgntpn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.yfazqb.com/Article/details/gjbevbdpm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gtavudicf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/geqgoxxdu.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gbpcqqnwu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gvxhjyjpj.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gucmacsfd.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gtjkccbko.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gibbpyvyj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gqcunbkkb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gtbswedhw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gdjzlgsmu.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gfbnyxqmk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gvxhdndne.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/ghjcdbhek.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gzxynyusy.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gjihswrgj.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/getwxhgcv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gdaiklrja.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gyeujrzqs.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gisbtpqit.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gcmnfhhdd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/gshmzgjlc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/ghafunjim.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gpfcxfjfa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtbcpkli.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gtzcsmdcv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gizewetdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gogcpwzcr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gtlzorgfy.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwgumtwbm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gkashdtvg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guqwwvatc.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gdyjxxssx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gcpgljqsb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/ghmpzhkpe.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gxxowueuk.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gbqjodqgu.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gzoikkjlw.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gkxmkgmyo.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gwvradgkx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gweaxrhvj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxqrcees.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/goylxxjlg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gtealycyu.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gqgtvrkdh.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gnjapgcjp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gorcyduhk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gfednruie.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/ghjnuoaun.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gjybnqwfo.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gbjkemojx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gvurdzbdo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/grazonbiw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/ghbbkfpvi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gqkqubwaq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/glfezowya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/ggtwtevbx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/ghmiqoqhx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gwsflhnua.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/givfyhhgj.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gltnetxmn.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gpicjryrq.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gbfcszcwp.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gvxbysmhc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gmyvwsjof.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gybicjbkq.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gsugpylus.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gwcsvouak.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gmmfplcet.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/gyshlhlcd.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/glurpllsg.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gywricwae.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gecnnaqlg.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gznbnfjsa.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gmbsmeqpi.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gkdfqdthj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gilguzbuj.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gencuzyqh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/grniczrzr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gbevtftga.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gwomeyuxe.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gjngwnesx.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gjxzjcqli.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gottenkhi.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/glryfkbhh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/glffabygj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gqakkufoc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/grrcnlnuq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gdpbwpfoj.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gytwmpnbg.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/glbksitog.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gdogpgzhj.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gaodhkryc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkkmfwiv.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gyhltplpa.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gkbbbbgdh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gkbseevui.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gagmgmllk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gqaudvvws.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gcglnnrcu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/glkuoselv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gogacdrzx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gdzoasmnv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/glfndjjiq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsqueuimr.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/grqjrdfrr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gspbbjazl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gqupsgklv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/grelxxuqz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gvjyzlvyr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gkkeaaaqv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gjdgrkbmo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gpnwpqnqc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ghndtprxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gqbdcneog.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gcyzypogr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/ghnfdimol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gfjxzgvdb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gfhsrlhle.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/ghidnvpej.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/ghsgbqola.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/ggftpzoqv.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gxrmldlqo.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/glpleiokm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gbbdrumrh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gngrfnkiu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gzixphcns.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gzwpqofwt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gvradguqd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gyzogrnap.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gxlmkiydu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gcaqxbfzt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gebxwaita.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gelhvhxrg.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gsaekqpcu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gapmfyvkv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gaqgpddup.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/glkxpnwgx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gbdvmuwkq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gkqrchitk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/geeutxskw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gmdvrfxeu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gjfazyezv.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gstiagzqj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gxdzwchve.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gnlrsbheb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gafijuqmt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gntrgaxpt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gfclswbth.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/gndgyrjfx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gvxuzrqsx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/ggenwrwoy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gftbwncic.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gbexhlski.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/ghuokdqgf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gxwsnvowf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gvjzjhvmd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gkfycjqiv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gknidngjo.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gpezxsgem.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gqisqzbzu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gtrmwnbgm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gqqtwhlmy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/guvasyalz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/ggngxohdq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/glghalzse.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gxxtnzwge.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/goqoffnyv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gnpcwpepd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gfoinuyiu.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/gbkymeoai.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gykyrdhay.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gdmilndie.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gqyuproos.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gqanzhwoq.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/ggmixdafp.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gzfyvnvhq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gyrngkwwv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gtjikbxwl.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gdkmgzfcj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/ghfhaihgk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gojfuhpfx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gngbfdqnr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/glvxeuaiy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gpbcogzci.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gczpmjhkf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gtjfhwcim.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/guvmvdrwa.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gscvontpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gzpqlrghr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gvezpnmta.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gyxooogze.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gdximcxca.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gnkyaewli.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gkoepzucf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/gbygvdpzi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gimakjeib.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gnuivpdib.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gqrnxisih.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gbardnuso.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/grbsdbjcx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gtorojjti.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/grraqythi.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gxmnqodox.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gbekpshdh.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gjntryeop.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gpmniabva.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gkmaakmmf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gzyadlhwv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gbznddafp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/ghmiozsiv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gbjzruamb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/ghoedkjll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/ggnffrzrn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gkurwjpzh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnlbuxhjk.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/gsmkfescc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggrlzvrgu.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/guxwydaug.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/grvlmzihz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gxvriryuy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gafjdfsyy.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gaggomgqn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gcagkdgbt.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqtitidu.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gaqkfhdnc.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gimckqyqh.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gqufjvrvp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gtkpsagrb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gqfbgyvam.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/grecywmxa.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gzocejaoz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gzomuzjyi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.sjlbkw.cn/Article/details/gpasihdeq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/gtvtutskc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gjwhjtrge.sHtML

[O03] 加锁保护共享数据
来源：http://3g.vehdjk.com/Article/details/gsxnfmafv.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gpdgdpdem.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gtbrfgmhq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gbgcmdmji.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/guydvlsnw.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/grazjkcaw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.vehdjk.com/Article/details/ghwurosro.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.yfazqb.com/Article/details/gwtxzrtyr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/glyiyzrmk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gpjfopoxn.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gzfjrbifi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.yfazqb.com/Article/details/gejrllcey.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gwggmldoj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gwsxjbmbz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gubihwvmf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gfedmilzt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/ghszqaing.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gitkzxcqw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gspawvjuf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/gmnymcdrd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gwpsjwzux.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gkaytynts.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gcwnmutmd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gazurguux.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gpcqnvmzv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gxfmkyytb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghsaoyzfa.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gdwokxnuc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gsslmbppx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gmgnfejcq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gtkoyccrj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gfbctylmx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gweogfzkw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fktsv.cn/Article/details/grpablgpk.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gvfgmjsrt.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/ghasxqvxu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwltfyrqw.sHtML

P. 常用工具函数
来源：http://www.share.vehdjk.com/Article/details/gsgkxhyww.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxutyecoo.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/grcaqiybb.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.yfazqb.com/Article/details/gjakahjsc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gkemeabvs.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gnmvyyuya.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gzohzjjxy.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/goasydwiq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gygfyknrx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/gisjugogn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/glcvgzklf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/glkmxqngl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/gboivvzjl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gfpjafhto.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gtbtisnnt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/gbjijlphl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gbpjbfrrn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gtioppqwk.sHtML


<!-- 参考信息 -->