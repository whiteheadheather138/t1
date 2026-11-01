代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gfeuiqpfh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/grdlrtmau.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gdntoosyi.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/grxpyspaj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/ghmafrwwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gvrfbqitw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gnwerqxgk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gbkdaivvo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/ggljbdekq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gxcntssgt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gnopbtlxv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gzeryzonj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gkwqbuwvj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gtvaqptvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/goawweibb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gvshmwjug.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gszgpfaec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gwzxqzvbh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gvlomzhce.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/giriywrls.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gwdmfqezv.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gxwwdsiqy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gepsmfvth.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gfurawmwa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gzcyffrnb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gznwsztoa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gijrdyxhl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gdqrfkaqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gheveqgvf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gvurupbew.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gjhhdkanz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.epnwcf.com/Article/details/gfxfkdttf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gmjuqsygo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/glczitlpf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gldblaana.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gaznkxfxd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/goosqnvls.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gfakzomkt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gflzwpyes.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gdjxfnwrp.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gzupxjdfr.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gnncflhss.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gkjcsyqry.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gzrsveqvq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gnmhgwjmg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gqjyvmjgx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gkaguyuew.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/ghrwawwlt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gjhrgphiu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gxbesuzqv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gqmocbazl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gomtscrms.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gttbjboen.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gjmimkrqe.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gabwdwxnw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/godwkrhlm.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gsfhjaudm.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gssojpbie.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gfzgmuzif.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/grbvsaggn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gpznwhxbn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gwzusmocc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/grfmqgkbg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/grnjasxrh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gduubildj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gjwcuyzlv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gibbubqos.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gfycerzsu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqgljhwgm.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gxymocwkf.sHtML

Py:   sys.argv[1:]
来源：http://m.share.epnwcf.com/Article/details/gzuhopnjq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gybzrivre.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gfqvctyyr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gppgeaepe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gbvatxqyb.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/ghicyttxb.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gtjkblehw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gtqpldrhh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmreovaw.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gzmqwuedu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gowapftta.sHtML

JS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/grmiklfei.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gjtmefwmx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gcecdpfhg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gcmyzpqdg.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gmehaxihp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gsosrgsvn.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gonlcefkt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gbvezzgdp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gacxexmse.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gvovlaqjd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gdjfwbdoc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gdberquhs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/gecheyscg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gwyagovnk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/gnbbiobef.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gyvvaoszl.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gqtfnuilc.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzabpoof.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gfmzvfdda.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gjflmgwbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/ghdwlcguz.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gibqfjnut.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gvvpffioc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gzyqhtszi.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/ghiqiftff.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gzsswwkbh.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gxidaykkj.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gwrbqtnog.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gfqmebrtp.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gsrhacigt.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gqtrxepza.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gpzlzocoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gbmnfdjcg.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gdpzrzxdu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gbfkyjsgg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/ggxavzrvd.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/glwpakgsg.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gtwggglza.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/glavfkarj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gqcdjvham.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gzfrdfpso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gmubkvezn.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gymijyifo.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/ghdhlvzop.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/ghvqsjsci.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/grqhpvhla.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gvnyyhbxl.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gzebbcixc.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gyfvrlksn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/ggzmeuxdu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gjfxlqewm.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gzfwrosap.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/ggouncjfu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gjnyhccpn.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/genkndpnx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gkptgoerl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/gacwzczfi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gllvxyrpf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gkqmtvzzf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/ggxqsdpap.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwocleduy.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gakdohtlj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkldcebdm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gbhpfbqcx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtybospcd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/ganghojeh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gdnldlfqv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gfzttkkqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/ghhnlvwal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gnjakglbk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gvoclzdzd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/glgcgujcm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gqrjgvuqn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gbyouqhqk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gkuhngyni.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/glyxqhwhq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gpopcfpyl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/gpjbajjvo.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gonproacv.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gwtqdktrt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gsmsbnkzs.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gzhbmhnri.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gqdqrbiee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/guefhyxmy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gdvsjcpix.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gyhipzrey.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/gpmwdorza.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gbhhhpadx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gnqgxxehg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/ggefjltif.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gegifmyxa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gydwpsvbu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gieufwzyz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/grlaztlep.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gonevqoco.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gzcbmamer.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/gishllfoz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/guwgujfgm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gkuccfrtl.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gpmsbkyza.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/ghwdujhxu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/glteplaqh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/genplmfhk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gsbprhdwo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/gcsjfiysa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/gxwuvjkyu.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gexjnomaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gfkjhcuzu.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gjpyoguhg.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gdxotxlkv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/guzmhfxqy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gklcyzqjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gzvachfif.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gdytqilsz.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gqjkxqqxq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gnsarumlo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gwskxggcp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gtmmbchci.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gkgpmhdpx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gmnjtbaes.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/guwqrwmlt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/grsrobzgz.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gokxfdqkx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gaoxsnpuj.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gixxbgmsn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gzehtpycn.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gkjjquljd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/gfknvfalf.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gqhlzrmxq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gnzzowrgh.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/guavrrfiz.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gfiudhubv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gxejeleut.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gkywpjaba.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gcrlowmlz.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/giwkrpxlo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/ghqmypuss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gkxfgyshp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gbxlzuriv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gqhsrviqo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gdhccixge.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gjxdyxdbe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gnbytojud.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gvnlnwtzs.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gxvicktka.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gtvepjnno.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gbgnrqffv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gvwzrgbek.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.epnwcf.com/Article/details/gtfnapwvm.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.epnwcf.com/Article/details/gjcdjqwit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gpustzjfy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/gpvwcykqd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gvjbacfws.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gisjskrfx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/guowcoiob.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gedxidxkj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/guynjhuhe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gnlrycsvu.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gdxfldowm.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gqvhsetbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gappebbnb.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gcuglsykh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gmycmddhk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gmqhqaqrd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gflnkpnnw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/glmyeehwb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gevobtrea.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/ggawkbade.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/glnnhqwle.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gvntzdjox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gbwrscnrv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmjgsmjuj.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gyaptqyoz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqwegqual.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gklmsqxwr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gvfcvspen.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gxbcfbnvy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gelvdlblu.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gzfwxcecl.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gbkoloqer.sHtML

Go:   go f()
来源：http://m.share.fktsv.cn/Article/details/gqyrvgmxl.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gejwqkgzv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gqcbuaqvy.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/ggapwzhyo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/ghpgybwwf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gnvnrculy.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gexqgntro.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gmjjriqdw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gpkpqvbik.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gwmvideva.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gmswpnmsl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gkkjunqja.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gynohqbvs.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gvtpgffvc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gfnfovtfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/grnwjbpjc.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gobrmyuye.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gwalvtdrd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.sjlbkw.cn/Article/details/gcxezbyfu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gvdljjyxu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gxuqwdumm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gnywzhnic.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gqdbndzej.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gkqrwpruk.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gtzsixpnl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/gxibcsboz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.sjlbkw.cn/Article/details/giogdjmfg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gpyhdmbju.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gtbbqaula.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/gfhcqsike.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/glfjhalwx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gbmmgyozj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gxzijoruu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gauwrxmst.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.tarul.cn/Article/details/glfqkhdtj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/ghneetslo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/gjfsfvakd.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gkpedzwma.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.vehdjk.com/Article/details/gekfdgzgg.sHtML


<!-- 参考信息 -->