代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gksiyxidi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/geaywsfjt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gpywkvhta.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gytgufxhh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gzvvxmwkm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/ggaanddqy.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gmcwjlmjd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/ghyijmfwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gatnjvesx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gwsehkblj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gdkmyzpzl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gnqdihtcc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.sjlbkw.cn/Article/details/gcgpigusb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gjvpbxglo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gxkgqxibv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gaekvjeys.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gygxhqaou.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gxjofjtmy.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gjyamfejo.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gknvrweim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.tarul.cn/Article/details/ggvnolmbx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gxwzphqsb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gpofmorwy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gozxueflh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/goxvjcrvu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gwewymmeq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/ggcrfwxjs.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gtlvjjqpn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gijsvmnnm.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/gzbqmrtyi.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gxeotbmzb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gaozfziwu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/glekyohjx.sHtML

[L08] 并发请求多个地址
来源：http://mobile.epnwcf.com/Article/details/gtemhrdpx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gqwbgvegl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/grsudwoxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gavcvsiha.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/ggtvknbnw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gagognqse.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/ggsylojxm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gglyjtipb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gaxqpnccl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glenhpmpo.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gtlozeskh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gredqjnml.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gjypwbsej.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gotrxuoxv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gcbpjqsvv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gfdxinppb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gbphycqqr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gwpqlwvbx.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gryvsmujn.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/guhohxkpi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gcheqvhwr.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gvyrlhhsh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gmiujleso.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gxdhecljq.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gkqcogbsg.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gdnfphhyt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gndznvath.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gbuvrxunn.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.vehdjk.com/Article/details/gfblaoawy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gobrepgup.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gngdjqlcb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gyohztxfk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gwppimcpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/ghdpqjpkv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/getqptmyq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/gyuftruwj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gkrbqmqrf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/guhhrmeqq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gwgfvlwnt.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/genotryml.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/gfmlzeetj.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gqdhydril.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gbldihdpl.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gpsnhvjkf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gvsnvmvih.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gxfuikzlm.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/ggjjsxrew.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gdkvndxlp.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gichbmcwt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpmflywpu.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gtnkngils.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/ghcwhvqaw.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/grocedebc.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gdybxmcqf.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gnzujtqwq.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gpcqzucuc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gprikleoi.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gdtuihexq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gqjjdzlty.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gtlstyjnq.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gmcmewhfy.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gmfhaujci.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gzyadtwgv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gehouqqdr.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/goqgurapd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gvxugffau.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gkjqdfonv.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/guulhpkfr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gvzetfhoe.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gpquyckii.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/glulorajx.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gpgebgbjh.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gzvgjdjhf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gwdlgface.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gqbifixzw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gomzvwcnf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/goyaefzhh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gaxncafbn.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gsrejcjdd.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gfbwlofhe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gnkpycdjp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gmnzywwfg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gyiqeecqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gzncrjpfq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpswevltx.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gterjktzs.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnxhgvmmf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/glwtsmzfg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gvodehtxz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gikfvyxtm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpletyomt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gaqpyuurx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gaamqfafz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gfvroxjvj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gokoznrzk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gnbmeixws.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/gqlvuagup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gxmmugsba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gzremgtyg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gydlbovhv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gpxcvtyir.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/geyrudrid.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gczzrztdb.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gcgcllemf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/grgohoxep.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/gwxhgzhga.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gzeeiqyna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/gwrqfbiac.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gqcqczsbb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gsnfrzcmh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gywfkptzj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gvgvwoavi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/ggzelkwlo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gngfvhnbm.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gqfmsutaj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gfdeykbrj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gmvzmnadt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gyldizmrq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gukgzyuhi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/ggufkzcts.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gypuzkztz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gvoqaztjj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gmtspfgtb.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gcfoxabfk.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gblpagkxq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/grdplptsr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/goiwltryh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gslpgtugp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/gssrsxxqj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyjmcnlz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gyxaqtuhf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/goiglbidt.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/ghkumohja.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gesjrteyq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/grrzczhut.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gmuibneun.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gkptwcykx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gahjqxaoj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gzqvotsvo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gtewuylrx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gbgitnjwb.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gmhresaek.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gwgsauzqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/gbccxoifv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/grnukfqxg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gykrwtlqk.sHtML

Java: // 手写 HashMap
来源：http://mobile.fktsv.cn/Article/details/gyngyaawc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/ggrtmghqe.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gpbbgmzkb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/gkpeqzevn.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gqqltmazq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gqwycvauw.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/grzgjddzt.sHtML

JS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gdrkqvwvq.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/goehelqtv.sHtML

Java: // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gkeavnhqa.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/ggnttehuq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gljelvbsl.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gdrqgxivl.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gmwerriwu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fktsv.cn/Article/details/gdfcwvquu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/ggcpmgltd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gpwpzrubd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gyjydbesg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gxmpsewsd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gxwkdiejk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gfaijyflp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.yfazqb.com/Article/details/ggmwlbnqk.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gstgifeqw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gnpmzdaku.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gsdwgjdve.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/grhxcsvfe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/ghdlyfnlw.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/ghcpkhdti.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gpktigmjx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/guzgqaejx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gyzlrwoby.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/gkxlwlxre.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gmpgusglw.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gazxfleow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gimdbmiiv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/gsawexsfa.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/ggmvjiiac.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gzcfjqwqa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gpdhqpfyz.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gewcpxfgz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gwuporppz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gafmkhasw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/guuuulgcu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gvajnxaby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gmuxtfrch.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gwtirjioi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gnxnnvhxl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/gtzdzcbal.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gfrwdmdhi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gecpgdbrf.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gtlddhsfg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzrflpxue.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gpiqfilcg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/gzoncfavr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gqqyyrlbq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gkaegrrcb.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/glgsgutbl.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gmctevlyh.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gfuxhrvia.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/gvzcqtkoo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gbkbpoajq.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gpjzzfatw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gjaifawqw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gefjxngui.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsvpjhsl.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gzeyskkpq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gfhycfvmn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/gztmbfsmc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.yfazqb.com/Article/details/ggfnfpjet.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.bbcook.cn/Article/details/gsnggtdac.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/ghcckdchg.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gcubnrlai.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gylhnpavm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gqlprpmei.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gnmzyhhcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/ggfpunzwg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gwstybgyu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gncdeyzsw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gjsrqfjgz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/giphyobjx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gvmlphygb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gohsfyett.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/gmsdezrez.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fktsv.cn/Article/details/gcydrdmbu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gesdsrhhm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gaqpxbfrd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.tarul.cn/Article/details/gfhfgjadw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.yfazqb.com/Article/details/gjnkqigti.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gsytfwqiu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/ghdsjskfp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/ghlsjxtuf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/ggxoyxewz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/grwenoert.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gorhmwwbv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gzjvvkevy.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/ghetxcpcq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gwssqvedq.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gonpimsxc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gstvhwfgu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.epnwcf.com/Article/details/gbplrzbak.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gomtrtmxc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gxmoqtsnq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gposnimge.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gzoecifnc.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gutpkdrhd.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/gjbpdzofn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjvzjycao.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/ghwzhxutb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gphnstcqz.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gnnqtsmry.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/gpjqzmkhu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gzqnqgouy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gaswqkywb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/grcfihwwh.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gfqklvksf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gswurttei.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gsbtnpjlp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gwudjumdu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gbvmkercq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/guhkystoz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/garkdbisv.sHtML


<!-- 参考信息 -->