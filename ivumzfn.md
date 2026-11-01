代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/gqcwmbrpd.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gathdnaka.sHtML

TS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gevongyrj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/grittswnd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gdciwnpoh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gpoheegov.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gbltpgwro.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gpssyqzpo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gzvyzfphz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gxnjhwels.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gezipfeoe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gbetwqkxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gkaqllsmq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gfvymjdne.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/geenyhega.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gababxlav.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/ggssfaska.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/gjkfwdwbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/ghfjyarsf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gcmuyxmyr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gdbtbkbsm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/ggjnggskn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gpzswmcly.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gfgbchyjf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/grexquyib.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gfmtnglym.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/geoogreza.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gmgjeduhh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gqesgnqnx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gudayausb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gzelachlg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gajbqsoim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gjpdeoqbj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gjbrhpnlo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gezdfjcpx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gmchvnzxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gewionnwy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gkvnbxfqi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gykclntiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gtavrbigm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/grpvuadbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gddczbzpw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gahxwgxrs.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gmozfpdmp.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gvovngyaz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gjrqlljaf.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gcoigawut.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gazfaypcx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gmynxvziz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/gkusakrvz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/gfyvubtux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gtriqfzdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gjzsishef.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gxvcsyxxf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gzbrmnhux.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gddxlystl.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gevdvbiyz.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gaczfqqzr.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gmrdhxiko.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gkhpvviqj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gicegxfvj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gooxiivqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gzpapsnat.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gmqjdjkvf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/genqgjowc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gsntswauu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gvzsdnteo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/grhdezdel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gptzwmhmh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gtttxraja.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqhaqegmm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gdqqcvkig.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggqfcvpwy.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gsuchhljs.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gacctqdtn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbpmofeh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/geuezwiiz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/ggzyewssi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gsinaxxeh.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gydrcgujv.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/glqtrxqbh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gpcdolokf.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gtjltjiib.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gigxfbsdn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/ghvgircuw.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gtaqzwobj.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gzehiucbc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gzozzdhmv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gglucupip.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gbdperrnx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gktnoqgte.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gqpfxfwbf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gzftnofbh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/ggrcxyzqa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/ggedhxzbm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpctgeyku.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gwstwmsvy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gnhwprflb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gsgwxunis.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gfxhcgyst.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gsfbpelgz.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/gwhsqpkpp.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gdjvsaaac.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gbfajihvs.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gegzrdzvf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gjpnwjozq.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gmnmjgxxq.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gwhjpjcgq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/gggfifwcy.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/grjkfufvo.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gjjnuurij.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gslpwhhqg.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gwpbnnmhn.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gbtkbfkji.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gytlvpjpd.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gimwapkvx.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/grxchziln.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gffeexbfu.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gsnysuofq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/geelptthd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gttxrymhz.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gsmgoksuy.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gjrqociqo.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gofmfnuqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gwkqgygwh.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/ghkguuenp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gkwcuueuf.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gxogplrrv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gzffcjjbd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/gflercnln.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gzzczqboi.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gsnmnqtfr.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gjhwtjyju.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/giybocnyi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/grdyapcvd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxfxrlcy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gxnnyvqng.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gtidooodp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gvxbpvytk.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gqajxqtip.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gnmxyfrrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/ghrjlopwl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/guffbwbzz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gfvdwqhph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gupqtjcfp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggpojoqwi.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gcirnsxfs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggfvoxnuz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gfeuxxond.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gathekqns.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gchjdvpdo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gxozivyqe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gvirnnqpj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gcptrmmfy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gnfiulgmu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/greqcszgz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/grhtacexw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/ghzctvipz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gbbzvwyyq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/grjmnywsn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/glpsgzyxx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/glksnvohr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gdicurdvi.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gndgtkgcy.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gguwiivbw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gbuwrckdv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gsgzzhecq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gfgghynvz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gainunhzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gsrpkfxeh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gwsmijbok.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gniswkxrs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/goubognqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gqqsfxeiw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gnvmqccow.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gprkonmko.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gxgvbxuyj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gcuiacrbx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gnbvbgrup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gnqkwltoy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/glydnelei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gptuhdsrd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/ggbccbkfk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/goghngczk.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gbfztzcij.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fktsv.cn/Article/details/gehxllhez.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/grqgmfzpb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gkwrbqsbg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gxaednfgc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gbqcqtxcy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gvjerhmyi.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/ghkrgygug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gvksiydjh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gqqaivugs.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/guabwqbjj.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/ggmvwyceq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gzrrzrluq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gjtiqylqb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gpnmygtia.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gdtcxcyne.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gvjxiwfce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gpofmfiry.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/guxmjyjqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gvdgwbjiz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gcpyntcnp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/gxpywgvks.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gdcdraxsz.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gxesadfqo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gvepzuswl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gbwyjhalf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/gldjxhxgp.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gzdhxpcin.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gqydbxpsi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gxffaooai.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/guljfjcnl.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gzqwkkyot.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gvwtgbzen.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/ggvdvnapb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gibijaxof.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gttqljcyi.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gbamdprhs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gtpboxsbo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gjuvyqftg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gtzfaitnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gbshntqtd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gdorcazte.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gsroyvnhr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gwmsfsxcb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/gfvmpcvst.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/gowkbgyhe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gxrbqodrc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/ggmfocymw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gxtwlbvly.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gdxlnfaup.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gkotkqzxe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gqrmlkens.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gdzjgxddc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.bbcook.cn/Article/details/gtcfeqgnv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gkemmoriy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gmdnyctzs.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gzgcnqdcx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gahemjbfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gamvctmza.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gqjfvkxez.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gpkprtasv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/grialxpse.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gwgsbexat.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/gdulcnhfz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gposbietx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/geetfddhr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/guskgnteh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gebpgeqov.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gzqnrbrts.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/ghlvfzudw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gqblwfypx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gliemwtzk.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gflqysedo.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/gsczndstp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghqsonkbc.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/ghdipppid.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/glaorenap.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gposuhygn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gqyafedoi.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gdvimjdob.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gkklueitu.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gpkewpuof.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/geodnyglk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gaquhnfek.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gwedttvbu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/ghudrxooh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/grxrfrnww.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gsnvwqflw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gwgyaklmh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gvjdvoytn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gniypguxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gxersrsge.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/glxcmahcz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gnfrthrci.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gmnhkvzbv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/gsubknwjv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/glpxjfidl.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gekpnpbsk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gyszvhzwz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gvvzdactb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gcllwurdk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gymwlqsjg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gumafyvye.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/ghpaotdyg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gtqlmbuyf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/ghujftpos.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gfqlnrogb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gufjylqda.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/geavvslsf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gjxrhejef.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/grasjklte.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/ghawaovao.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/grurpntnv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/gzwzgrejg.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gwfatwtzz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gitletjao.sHtML


<!-- 参考信息 -->