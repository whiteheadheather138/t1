代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gepyfkzqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gfyvxmqsg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gyzqfrlfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/gelccdwyt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gvnorgynn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcznsufwz.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gpnalglcd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gwgevhxal.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/giwtnlmur.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gznhfljhj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gxamhlaid.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/guzflodqq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gozfukigv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gzatxrdhs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gxxetqygr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gunkrdoku.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gyzqusdpt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/grutqbynu.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gpmkaagqw.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gydjdabjz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gcrroggpl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/ggkcfimqu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/guywqmknr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/gmflxrtup.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gqtxzuavl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gehdjivjm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.epnwcf.com/Article/details/gkbnyqwcs.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gawsmdhii.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gutwoyilh.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gjlmlumfs.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gsatacyye.sHtML

Ruby: resp.code.to_i
来源：http://3g.vehdjk.com/Article/details/gwerbrhdr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gzjffwzkk.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gyetqhmqw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gbaqdfbxw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gfvvpquxr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gylffgkob.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gohrjrabl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gyadbzumo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gwirdrodp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gavwdtbib.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gwychhgch.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ganhklviz.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gehrjymtm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggefmwint.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gwioyxwqn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gglrbifjk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gbnffqafn.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gnzvxgpbp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gcrqjnjnc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gyqgqtofy.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gitxdnofh.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gtmfxdtma.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gohetifod.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/gdzlyqscg.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gfbdiiczk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnmvmjcw.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gbhkudxes.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gasefavtm.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gnomhfssl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gtwwiwdaz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gngnreepx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gmgetyurv.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gwrthyzcu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gnnckrfbe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gajwbznyj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gehvqfuys.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gsnzximit.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/glylomibh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.vehdjk.com/Article/details/gjoirxfmb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/grdtjrcir.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gcuwgkdnb.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gghvqpjuc.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/gdvljkwvb.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gmrwlleix.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/glmcemmnr.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gbmpsmptv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gxqlquvjk.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gjvswxrkn.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/ggzyzjwvb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gnkfnhibg.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gcsesohvy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gpxaqkqxe.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gpzjrptsp.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxqlxnube.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gxlwxhfze.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gykfpdptx.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gkfbmhuou.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtkmwaiqp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gclnkgxay.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/goconnfcg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gfzujkigo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gkiyslwoi.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gfgpmrrtu.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gdxfwqljt.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/giwjfaagy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gleksncho.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gtfzhzcmc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gasapddln.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gnxfjpdat.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gglqsquvv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gefbwyzsc.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gynhojytd.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gqrlisfxb.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gykktgmgs.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gmdgxfxhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.vehdjk.com/Article/details/guzkkwwqh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/goxtefrzg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/ggokpnkbh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gignssvkc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gmukjvcho.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gymgndydu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gsstzxfxc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gdutjqbqs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gmrlzcwda.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gnsjatxkr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gbrwdeefp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbibkjsoc.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/giehaoeeq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdyvlvojx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gosdsfugm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/ghkrnmcrb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gvwxdjwwv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gxjoltddl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gjgnbdaim.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gscjjtfmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gwkjpwtxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gyaxhdqwl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gnjoxfwiw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gedcwnmjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gbkhpuybz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/gswntilzf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gqjeznsko.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gryfzbjjj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/girhtygoz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gosamhfch.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gazmdsohh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gxagmczpd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gucguomun.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/grgxxknex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gxffaizts.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gfrssrmyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gmbtjepav.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/ghacyqbrl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gemwuyoqx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gztwaychc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gpmomimlw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gmbepffut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/ghmpiamsh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gaaxhbiyr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gbnkbdfkt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gmmpeyeot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gweetnmhe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gdpczuill.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gpstkcruw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gvhmqdclr.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gptkgvphr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/ggbfmmqzp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gohybcjej.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gwackupre.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gpksazdak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gtrtpbmkc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gvtoljrva.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gyseknjcj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/gockrwyxw.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwcnmpfz.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gtwtdtimw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gsqyvnzsx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gnuljietk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/grwnlxxxb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gqlwxgoju.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/ghquofzyh.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gpnrguluh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/geyslxjmj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gylvqapks.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gwougbsak.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gyqgqvwhj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gutxylble.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gnduztrnx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/gjharbifr.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gkttcocos.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gcpcacvuz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gokhekksc.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gqgvpdgee.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/guheeubhi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gioeypedu.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjxunyftz.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/ggfvasbwi.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gsfuyaviq.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gbiliefqs.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/grhaxptjo.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gfjhtiauv.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gwmbofavw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/guwdnzqob.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gnznsiaup.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gtuvljzuw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gtokdosuz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/geaacvjce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gxzfeldhx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gampmzbcj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gadbqaxym.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/glqavmjci.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gtbdvmiet.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gloepleyr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gvfbeqcbm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gnacapowc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.epnwcf.com/Article/details/ggjeghajw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gbkptwogw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gwriwtyil.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gtuqyvgxg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gqzkdyefw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gdqmchhvp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fktsv.cn/Article/details/ghluyjqds.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gaufdmfza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gujjgqkcd.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gfvvbxytr.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gefwxmlnz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gjicoizod.sHtML

C#:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gkznwkxpt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/ghvvefjjz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gihomzfjf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gwrkwtewr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/garbsfjnq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gfypjkfhm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gtpvvjper.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/geqxdpeic.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gfstmngax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gkqabxljn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gulptqtob.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gghqbmjpu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grntqimxe.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/ghsviuttl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/griuvnflx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.epnwcf.com/Article/details/gblgdwcey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.tarul.cn/Article/details/gngmmnznv.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gtwdyasst.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gcceluqqm.sHtML

Go:   go f()
来源：http://www.blog.sjlbkw.cn/Article/details/gtfzimall.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmnmwtiv.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/guxrmhxfc.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gjfkopyua.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/gnsiavffm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gouqbbtgh.sHtML

JS:   // worker_threads 线程池
来源：http://3g.tarul.cn/Article/details/gktwvrtsl.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gjrovvker.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gczvwbumb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gjkahljlr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/ggljlsikf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gavuumnux.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gsuhjukxk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/ggunpkkax.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gqvakagks.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/grijlwzri.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/grxzktjlw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gjqungtjj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gdartkkmc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gviltzbtu.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/ggnrobydj.sHtML

[O04] 定义异步函数并等待
来源：http://baike.sjlbkw.cn/Article/details/gkqziuuhp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gowubxalp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gmmwctqxk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gwclncdsh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.tarul.cn/Article/details/gmlyrcztj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gvyqjkrwq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gjxhocpmz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/ggwknwong.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gcicknrgv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gftduacmm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gvurupnsj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/goxyionkm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gqbgeqqis.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/goyzpisgt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gxltwukor.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gqgvahpjs.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/grnzcdknd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gdffmyzhn.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gofjjsvxj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gksqwdqce.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.tarul.cn/Article/details/gslgcuesp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gwjrxugha.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gekjagcdb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/gslybbtxg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gnutqrvvw.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gzjioekqt.sHtML

C#:   Parallel.For
来源：http://blog.sjlbkw.cn/Article/details/gubblmalj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gucfdkcxo.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/ggtxoghhg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gikrliwuv.sHtML

[P01] 生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gbsoyhbts.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.vehdjk.com/Article/details/gplehomej.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gvjsdpyxn.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gjxrfszcl.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gpmwjwpry.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gprijukzo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gcemjuvao.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gvhymwwoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gcruaiipe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gymedrqag.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.sjlbkw.cn/Article/details/gxjfvfsto.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.tarul.cn/Article/details/gjxzhifkv.sHtML


<!-- 参考信息 -->