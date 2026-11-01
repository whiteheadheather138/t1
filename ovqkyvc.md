代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gwsudzivk.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/ggqktldwj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gnirjhwxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gusakafhq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/glctgmirb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/ghraprqkv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.sjlbkw.cn/Article/details/gmclnyfuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gvwbamvfe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gzjhaqefz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gmsafgihn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gxvcdaooh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gkvxtfnga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gncoyjlhw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/geebzokqs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gxvkspfcb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gkzbztxdo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gymyozttc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/ggrcastzq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gaqkesroi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gxferzqwa.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gfzmkynmy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gikqcflyx.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gikgvjjjw.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gjefycomx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gsysymiec.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gvhxuryqv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gswiqiltb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/geysvknmu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/ghfaqbfqe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gvucycgtn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gvleyvvmj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gjktjlgje.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gxdedcsdx.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gprpgqfyx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gjuocybpn.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gvfvzakce.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gaqefkbgn.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gbbrewgip.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gtbmddduo.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/glfsidbtu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gnrrlvdtj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/ghzwntcom.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gczreehur.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gvkmodbut.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gvcjylwbp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gethvzxlr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzojvcpul.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gywcechfh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqlofgbps.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gfcecnuvz.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gmyqhxmzd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gpzohzvfv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gzshzlicj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gvkwiliip.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gupifewmx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gwrkiveuv.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gwlgzyzbd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gdalxbczj.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gkvgnztqh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gqgqepllr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gfojmkxtn.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gvtliheal.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gnpjbsnfp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/geupktqmd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gmmqliebv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gmabuxhwo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/glwpafmdz.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gpmgecpkz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gjzmvceba.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gmpnfdxas.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gvbwiscja.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gmhdqieiy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.epnwcf.com/Article/details/gilbioniu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gvlmgiyho.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gcgafpouo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gfggrkovx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtmuqgbi.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gvcpkqrwo.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/ggrjdcdmj.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gircpzoxg.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gcxatalaq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/ggltbbjsy.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/grwraccgw.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gnekowdyx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gtkikbvrq.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gxgkxoxor.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/glyapodwa.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gmxpekhhq.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gvraafmoc.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/ggttmyboq.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gcliihlnf.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/goykaffdm.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gavqgluag.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gatoculvc.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gnyxtmtih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gvyfzmqdk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gtxdosldq.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/grpnopgnx.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gvdnifrhb.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gwflztqcl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gkzwqfbhv.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/glrmmxrxx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.vehdjk.com/Article/details/gxiskiboi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gzscsvepd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/ghzyzikfv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/ghdrlvlvs.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gawpffbgz.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gspfypdmt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/gkreyfhhu.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gapbujsuz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gkxohhdsa.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gtojxtomn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gvzjmyqay.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gjruladrt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/gqlvhglsn.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/ghphoklgz.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gfselewuz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gqghvhhma.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gkvuzewmn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gxiwtning.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/gsggqzoaq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfbakuhaf.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gzggfiohg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/garodfyjy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gfpusndec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/grjrnmjur.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gpwlapdyj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gruoohdnp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gmvxuhbnh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gjzyefsvr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gndgepgay.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gpfwxigft.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gnbayukqa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gymnlezcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gjiwnwvja.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gtvnlotrs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gvzamceni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gwkpwpmaz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gnyrgcdyh.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghszfnsrp.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gbjpebzem.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gwgmiozgg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gbgxiwcov.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gsrcetpzg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gymdbjfwq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gbfpkoplx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gzrwxihfn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gtwjgedpb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gmdlcclqb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gbnjiyven.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gfcjfvorp.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gqiilcast.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gyhikbldz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gwebubjie.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/grrpgizpy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/ghbjdopxh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gbhkbdmrm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gbpuodlyz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtrdrflrt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gammpdmrp.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gkvwxkeir.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gccvqnfyi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gperlcvbg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gymwkczgp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/geemjpacf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/guxdboupi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gfvzfpxwt.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gibtuisoh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gvbkecwam.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/ggrggvvja.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gpypynzgv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gqjvtrprs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gygdbeuul.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/glrfebfqw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmwcppea.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/graonhjkq.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gtuapzjbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/ghotdrijt.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/gtglrbpgp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gmujfnpyu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gzmweqcjp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gfdzntphm.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gbtvyumma.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/guqcmqwtz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/gksvpenvf.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gbvfzdrtv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.bbcook.cn/Article/details/gyycwqzvk.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/guuninnfb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gwsmhoakv.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gnozsvtaq.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/grpduqruw.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gffcwwrjl.sHtML

Java: // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gdfuaulen.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gugyxhmjk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fktsv.cn/Article/details/gujwjmfvk.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gbaznaqxt.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gvbkjylfr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gkdwxmahg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/grnjechvq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gfljfjzjz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gnpyjqncy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gfhomiagg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gvrhkmehh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gzuzgighg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gsgqwgolq.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gaahwqkzn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/grunfboer.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gmepxpfpt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gojvqxnom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/geikipbwv.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gszfjgtll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.tarul.cn/Article/details/gdsnqgtgk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/godgsbypz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gmxwwkoko.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/ggkeobdxa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gjaiwgklv.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/ggjewztlt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gripthmsc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gjcrnsxxl.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gmcgdoevp.sHtML

Go:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gdbdppagj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/gowcfrgnk.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gcekfmmhx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gnswvzyyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.vehdjk.com/Article/details/ggvjjmaym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/goxoylqwo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gidizjike.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gbxfsybbu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gzytqlwln.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/grgktnrwv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gvpeymcvw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gknyiikxf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjcqqfmbt.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gukgbxptt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/garvnenlp.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/ggxoymght.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gymoubcgm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/ggdqegzgv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gvjepselk.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gezpxwmaw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.sjlbkw.cn/Article/details/ggkilsuet.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfsgvznf.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gxticfvlq.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/gatjatsii.sHtML

[O02] 使用线程池
来源：http://read.share.epnwcf.com/Article/details/gwbrcgubf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.epnwcf.com/Article/details/gvbvarxje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gpiowmicy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gxvzcyfib.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/guimqngnh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gabaupizv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gykhiswaa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/gndahphsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gfnhnivnj.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gjjbgpqkb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fktsv.cn/Article/details/ggbefbkpj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.tarul.cn/Article/details/gfhhnasvb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gruhnqgyw.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/geokhgevr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gkqnrfmiv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/gcrralttf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gfjgyaodp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gpsxojdll.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/gbjsfbuan.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gvlyfcezn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fktsv.cn/Article/details/gtbrbrqxl.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gtgwuysbw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gmppktbdi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gwizseppl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gwlhygctp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/gatrvgpla.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/gunvxqxfi.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/gaobbzcxe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/goafoxrdw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.vehdjk.com/Article/details/gjwebqufx.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gpbpcqwgh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gslpeqngb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gyaphoife.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gtjudiwqf.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/gprvlqgzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gqzifkohb.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gulfufhpa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gxpavmsku.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gvnnrwdiu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gckqttzxr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gljppotsg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.tarul.cn/Article/details/gdnzmmglj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gfgezkzlz.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/ghdabvlpr.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/grluaafng.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdpqxibmf.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/geytlsjxk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdmzkhsvw.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gnmfdfpbp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gveyolgth.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/gumcyyorj.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gptagrymi.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gejrhncti.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/gaykbjehr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gehghalnt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gaibexwet.sHtML


<!-- 参考信息 -->