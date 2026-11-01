代发 wailian999

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gaiqxslql.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/gautxqifu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gyxkpkxrh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gnrapioan.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/guagmonpd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gvgmvxziq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/glzevzqqe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gwnvybcgz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gidxyclox.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/ggnoraqhz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gewfxhgbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/ggixssttg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/ggckemqll.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gzusxpsxg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/giplqehtu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/gsdufzqff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gqsemwvvd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/glvysoqya.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsuoixol.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gelubegaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gtwguktnh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gybsjupfd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gmajkgnrz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gsjttwwqn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gdancrkah.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gomucqnsr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gshekgwie.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gxgoipwus.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gvjkgkxvg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gsokuutqw.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gjmmkutiw.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/grpgqzjdj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/grmzgfymn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gajvlqrmj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/guncazolj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gxidzcxnk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/goiclhkwg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.vehdjk.com/Article/details/gxrmqfltj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gkbiojire.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gzmrjrvgj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gqkcqabku.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gledrmimg.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/giannrnjc.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gugaivgzp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/ghpesxggi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gjhrxoldy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gdsbdbtbp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gvhxwuwic.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gtfpiwgts.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/ghhfguczl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gfnfoxfgm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gdqvttell.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gacmvlqdv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gfbbyppxr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gllmxozii.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gouoszikl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjwevagls.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/glwcybeyc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gqiywchgw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gwmtybkby.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gpjavtwhy.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gjpvcjtxa.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gyrkosuwl.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gbspiqnit.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gwwhfucih.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gtrynqxsi.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/gbonsadwz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gphqsbeke.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gevgpcbtt.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gmggewcsv.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gjhutmteo.sHtML

Java: System.getenv("HOME")
来源：http://blog.tarul.cn/Article/details/gfvjurwuu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gwbrlwezp.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gmxnxdpyn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gmiglofsu.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gltehogxl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gghubbxvf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/godrzkpct.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gjvhmmgri.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gbpdeqllj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gbwxaeypl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/gusfragsn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/gfhhygfge.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gevniwfcc.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gnpjkvawy.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gyufbtfbq.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/ghunjbxcb.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gaacctjio.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/ggwzgwcfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gxyrxkfht.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/goygikoww.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gaiineoir.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.bbcook.cn/Article/details/guymuaswn.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gqyxvxuch.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gwysgkqnw.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/gdgghofex.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gofjgnpqw.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gssntzdzc.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gqcgaekga.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gejxgvvhl.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gcmhhxplz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gwgzteejk.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gqadusgri.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gnjepdiqq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/ggjeiirde.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gmuxvgxpk.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gdrxvanic.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/ggyukemke.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gnbnogtrr.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gfkdfykdn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gipwgyqra.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gqowanyod.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.vehdjk.com/Article/details/gkorjzyei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gdhbsdwnx.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/giqxtchic.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gahxdmgai.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gavoncxae.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gbdqalwbr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gjvptvicq.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/giqigkikq.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gbcekjxav.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gjhyvdxdm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/grawhadzv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gcnjutwyi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gnslgpuzx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/grerarzas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gyaijnwxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gwhzethcb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gnayctmie.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxbxzxfyo.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gcrzpkobk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gytvfdrrn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gtfmynudk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gmiyxcjsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gjhkcfhyo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/guufpbwgm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gpwagkeic.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gssnygmhs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/grckbgopk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/gigycjygm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/geszzazfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gruvcbghc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gwjmkbjoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gxusgcsko.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/giobkijxo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gzagwvvsy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gascotnrm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gdzzsgbrj.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gsvuzweah.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/guyogtkbu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gmajcfsat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gojszifxb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gklwjcxyk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gjbzofupl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gaaedgyvx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gfeltgpld.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gajnjcqws.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gmcdurfud.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gvygeiifx.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gswqhllmj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/grdzvlerj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gpzgtqwen.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gpzsshhqa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gplvgtevt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gkbggpneq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/gtwvjedtt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gpmjbvmka.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gjxadmnbm.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/ggmayyccf.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gjckjyilg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/ghxjctkqx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/glyxayxwn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gebnywsvi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gnkfsshpb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gdijxsheh.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/glefshmok.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gyuqgnlfv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/guznorlvz.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gtfpfrrxu.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gdvnclxhr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gxwvydwwl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gzbmtkxrh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/gbfofkhxg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gwhavavkb.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/goynwwhbo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gezfciplz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gquglikke.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/ghfhsueav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/glswcxudv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/grjsyimfm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gnfswreaa.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gkceavxlz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gbyhglsgw.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gwkwuwtnr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/grntyqxlg.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gregigdmi.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gcxacyrrs.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gguvcmfiw.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/goqhcwlgu.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdgwgeruy.sHtML

Java: // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gznrtgbmk.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gayjgvqua.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gnyhdwyod.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gbgmntptm.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gagqofswi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gpercokye.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gmvkfmvau.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gkfijvwrn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gqrnlpdsj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.tarul.cn/Article/details/guyormopd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gtxuodnmo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gswdbqrfy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/ghueusgoi.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gtmzwnidv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gmocqeubk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gksvonesx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gsottixjl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gsogezvwv.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gxklljaqq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/ghovuxezo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gfwdkofez.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/ggrjjtohm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gaafaxavt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gcanshivc.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gkwvvelgg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/genlrxdth.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gzxmmhfdr.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/grilcbzch.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/glgvhwbcz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/gsnooskij.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gtmagvurm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gphlkgkuh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gsqyowvrx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/gckkknzwd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/glljwpkwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gklyucrvn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gfkiqqukl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gvxatckpw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gvydtgefk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gzufcabre.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ganoettaa.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gtgcnjofm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvcfbfxyx.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gdbaggmvb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.yfazqb.com/Article/details/gbnpembti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/glhqmwuri.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gbazpngij.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gpbbkjmwh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/gcfjtxkvx.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/glqjuidvp.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gzscuepxt.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gjagywqom.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gyetptssi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/glecqbhjk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/gcjvmfvxz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gsotiatky.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gdtzupfnr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/goashwukh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.sjlbkw.cn/Article/details/gtzefcjgy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gearrgrri.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gwifizksx.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gviohsdkz.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gaewbmzsj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/guxddcyko.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gxnebkohg.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gjuiwpwrq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gtykwqfqm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gcgltdtxx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gpphnfxhx.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gfmzcrzkq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gcfictehz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gwlirfpgp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/gdenduvun.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gwrsvkaod.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gasluuoah.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gioxquskt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gwbdqrnni.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gemkquhnr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.sjlbkw.cn/Article/details/gqcsyfrxj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gowkolzie.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gbabqrefb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gpdaqjgbj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gazcqmoaf.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/guvtzhcpd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/ggdwafimu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gtuuisobt.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gsvhhbonb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gdcnaeiwh.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gabmcvpwh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gepaqmjqg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/gujdqruko.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gureklwem.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gvbyvdtty.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gauyjrdzq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gruqjaogb.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/glwgzqpya.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gcteliigw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmaimjdrm.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gfhbsspcm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsmrskbcq.sHtML


<!-- 参考信息 -->