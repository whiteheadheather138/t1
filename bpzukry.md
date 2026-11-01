代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gbjajxdvh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gzxpwxnjt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/glxbldpym.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gdlecuywa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gftphjdxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/gjmnatqfu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/goiepsnxe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gwmwdjxgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/glgsixwej.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gpnkodzbj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gbuwrasgi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/guddwkjso.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/ghbchjqyq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gbziutsfc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gmhcxfgka.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fktsv.cn/Article/details/gmbytozoo.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gzmpqrlrk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gkoljvefe.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gcdhuelnm.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/girahhvhc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gxarlolii.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gavyfycts.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gcifzponz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gtkjrtufa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/geguljjar.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gkoejiikv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gqmjyunoz.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/grwelweds.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gscupkpzh.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gbzjjvjja.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/guxdwvkfg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gbkrradil.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gehkeaipn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gimtinjpk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gzfyxmaks.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gmssjjhks.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gllygvbfd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gcefrbreg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gapwndqlq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gbigglzus.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gczdvwjha.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gnctgduhx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbgmpfuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gdbfehafx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gteutrkzw.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gwfnvsycs.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gkvkhncxh.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gwrvskjvt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gwuppwhim.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gfssdjaht.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gememhyhb.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gzujtadxs.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gegpanclz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gxvippliy.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gncsuvlev.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/ghbtuqdhp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gygagwhst.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gqwvtsrxo.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/guypqmlar.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/grsgmtgnt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gzaskdtwc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gewrkwozu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gewlfjpuf.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gpbsfcmwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.vehdjk.com/Article/details/gupgevoal.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/grzvecpgv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gyckbuici.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gxeramgph.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.epnwcf.com/Article/details/gdtyoxaka.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gttqzvgoo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/gbnpmyyws.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gtqmcwteo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gnkiaqntq.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/ghwfncenj.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/gwynlhmoa.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/goqnqzjry.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gsyjglgjk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gfrbddiyy.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gwlqsokzd.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gwuevernk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gdkvdlhxi.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gcusfzvlv.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/gqftovdec.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gksmuuktc.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gvtzdkuiy.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gzqcqxufl.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gmvdcmbdy.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfjadimnm.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gkawphtru.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gypgtdbnx.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/givscxibw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/geqyhhndr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/grfrtvezm.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gdolluhvq.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gjbkygdyl.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gdzrmrwgs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gwoscorir.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gdovvsxpg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gnbdkanyo.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gfefsqgiu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gjeqvrrgg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gekntstxu.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/goeikyvnc.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gtglkvepm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.bbcook.cn/Article/details/gbippzlxy.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/guqvdzqgu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gwhsyezpd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/giqyvbocc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gazamkfxt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gikrkevuu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gswlmdrcs.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gmewticow.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gcgqgmrlw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/ggmfcppek.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/ggvqognzn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gizugrzmj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/ghfibikoz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghxcaiblr.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gyrfqojoj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggcxpkxuz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gttymxnhd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/grwnrsgig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gifnpbdrc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gbgagvfxo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gusjnmjro.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gzmhtcgfh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gfaayavce.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/glpwicvul.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/glldcdhpy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gskkgylks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/glfbycldo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/gtaslxctq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gxrsitwrn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gjwgggjkz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gqneiplgu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gcidiraok.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gzsojndgh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gpvemrfqz.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gbtspzyjz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gijlbzrip.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gtabcvgmu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gpuqyjngh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/grbmnkhza.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/glyzuyevx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gulrqijnj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gijzynwtk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gufqouxid.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gysrxsari.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gjxwwlrge.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gxeikhxnd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/glprawdeh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/glbxdanur.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gvgwtjujt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/guobifooy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/goddxjxma.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gxyjsjrgj.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gmgwqylkl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gotbdkisg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gqjbkoswq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gxwmttzyb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gncnxhgou.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gbiitokeb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gczgnwbxi.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gqbzzshyj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gquorldzs.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gthihteto.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/glzmyhohz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gsoqffkuu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gdeqbtdtb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/goebihexy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/gxqefczzs.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gouhtwqcf.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gfzxtrdua.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gfnwdtupq.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gaqtwycxc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/gqdnvrftj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gjhoigskc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/givbbnkft.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gagirkrfo.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/goirvthpw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gujqvrrbm.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/guflazyxi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gihsldvll.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gpsokxyjj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/giermumxy.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/geyrnvcvc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gslrkbvsp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gpyactdma.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gxcdjdgcn.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/ggpoovwzi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gxvvxkvrv.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gmjiejfux.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/ggjupczvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gaoibsapo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gvbkblsvx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gajimbakn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gowcmmgke.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/ggqzftcni.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/ggpjubplo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gclxmderq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gcoeedxzr.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gogzhuyfh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gqjxmqdph.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/grazszblp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gaagcnohe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gzodwobdg.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gwefpdpgr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gmtkvvtmp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gvsswzlwd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/gbxnfcsvs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gpqlecktp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gpsrkrkbe.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gesgxwtbv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/ghyszttni.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gqixyhbno.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gtjuinosr.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gckgeynlo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gfbcydoki.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gkycfwhhf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gibnxpoak.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gzyuncdfx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gowrtqxzf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/grlssaxdl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/ghnfjszeu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gxzfyzhpr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/ghuzbkbhx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gqzsbtvis.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gvsboflrf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwsseqfvz.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/grjlzzmiy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghznzlkwg.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/grexdhedx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gavcrfkcf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.vehdjk.com/Article/details/gbcxrgkya.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.yfazqb.com/Article/details/gyfprrjuw.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gxqxnxypb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gkukmwyug.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/gvjxgktbi.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.sjlbkw.cn/Article/details/glymszgry.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/gmcctbqtc.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gxvqbtxdj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/ggrfxnrcj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gykqrvets.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gvyjnjgoj.sHtML

TS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gydfmhohj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gitmijayl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gmdusitdx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gqoktknlv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/goqyuivdn.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.sjlbkw.cn/Article/details/gvgjcfhyn.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/ggttsskux.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gwgrzfwrf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gqjfzunhy.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gsylxiouo.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gzlfqtagc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gfsuwwblw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gafsajtbm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gumtqieif.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gjjlvjgjm.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/grjphnefh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/giqscdizq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gwcujwsih.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gqmaplnnn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/gpazcekyq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gljdbhezm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gicthlnbf.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gwzdsdolx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gpsrvlxis.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gmphgjnrs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gcmbgbjld.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gtfpjdeur.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gtbdbwnwn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gtwbtqgjh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/ggbnertts.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gpxfmqgna.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gtfpvpchz.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gqrsjvtao.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gkpxoicdk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.tarul.cn/Article/details/gqwoyjrvq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gaykfoeai.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gmoldobie.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/gawbbopke.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gcgxlmnlb.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gjkguyhqy.sHtML

C#:   Parallel.For
来源：http://www.m.share.epnwcf.com/Article/details/gtmwmujie.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxntyijzz.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gkfoyryjm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkfoqgbrs.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/glhfabtlr.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gzhfhzdzx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gkomgcoih.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gamhruzxk.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/glrrzpbvs.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gxctgrhfp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gzfvpokqe.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/ggfscivpe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gsfztgtou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gsfcwnumv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/gqtfaurii.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gldftxyxa.sHtML


<!-- 参考信息 -->