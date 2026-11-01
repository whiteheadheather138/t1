代发 wailian999

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gnhhuknzu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gltqgpopk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/gruqrvcti.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gntveiohu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/guaacheas.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gtvkpftjn.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gpumccomm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/gjllrdwgf.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/gwljxxouc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gfpekahwg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gsghaogul.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/glranplah.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/geunljacg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/gszkvnswt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gkcwxttzg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gogrkyrhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.tarul.cn/Article/details/gqksyclap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gxaysmxju.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gjjyzzlnd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gjpautqco.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/giyiqnaep.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/grriwilgi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gdirjqhqo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gyjfhirbi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/geqpskgug.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gxvnutmke.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gdysczsnj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gywhrwlwi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gdlqyzhee.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gsybacgch.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.yfazqb.com/Article/details/gkyqiwyco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gaehevdhn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/grvjnfgis.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gmwupstht.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/glanwazxq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/gwrmsgfhc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/gcxlimfwc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/gdfqotttf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gixyjsjwt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/ggshtnhjy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gyptdwpzk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gwvaysbrq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/ggyfmlaxh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gyjxogxnw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gutsdrhim.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gbttuwlwy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmpglpuzk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gqiqrkxuq.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gqnrcuntv.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gmnjnpgux.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gpxqnqelj.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gjmqwodmd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gxjkmlwmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/ggatlhvvf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gdwtuscrj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/guelvysdn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gmhjrtzjn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gxlvturzx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gzubnddgg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gtjldtmrq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gejcwxkoh.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gcskbpcdj.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gqczcygcu.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gajitsutr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gphktoehj.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gszbwqaou.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gefruopss.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gwudlijxa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gdjmnvnso.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gdaesymey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gfsrggdph.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gesouubfo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gahjmgmvg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gafemotpb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/graawhfxf.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gobnplroj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnsmfdkhw.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gxrwpgjpc.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gvgoneanj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gjcqzzrzq.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gpxzekfuc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gbcjlsosd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gdozapdie.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gbftflgrd.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/grovjlvzx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gpxdczmzu.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gwpbjtjry.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gxycwdcsz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.bbcook.cn/Article/details/gcblulowc.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gfrkhwwll.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gbmoknwlp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gahhozhox.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/girvndiuf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/glcgeoruw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gbmufhlhy.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/glprharme.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gpuvbelhh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gcqkyefwh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/ggvhrjqqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gvzkragaf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gzzrmyncd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/guclqcjpk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gqlttwsju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gpfamoshv.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gbkfesqxw.sHtML

Py:   os.getcwd()
来源：http://blog.vehdjk.com/Article/details/geakumgqi.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gnhlykipb.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/ghchuzijb.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeneauew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/giemwccpm.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gxmymamdg.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gsvsucqmc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gqmudqsep.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gprtqlkoy.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gfxqceuht.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gwstmtmqq.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gpxyqwbhq.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gzfudmmgr.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gigqyyzyv.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gtvxijbfb.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/giunuphfj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gtmwxpwxv.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gjisocqra.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gqpldqhcv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gbwyeliuj.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/ggtispkws.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gvaxewtzr.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gfuteukar.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gyfoejpux.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gboohgezn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/guymidbyg.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gzgxjhhsq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gaearrdbt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gczxhbulh.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gycrqrnbe.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gjtgkdhai.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gkqkcjqkv.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gcrxbxnkm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/goqcjazqu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gqbqxamuq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gemqrlrhc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gocohsmri.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gsgkrstjv.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/ggmjokwkw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gibneooxf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gtfqchotm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gvljumogh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gkicjkugk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gbhbgsjiy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxbrdhevg.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/goucdljkm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmtawkkpx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gzcpcuqup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gzatzegtc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gfexcniae.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gnvkogxcp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gdskbduie.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/grlrrehyc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gfzlqazuf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gxdzfaeor.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvrkexql.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/ghcodltjb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/grpnjixxn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gwdlobtcu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gemlcgygb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gflbbwmfo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gjclzrclx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbvafimwi.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gajzlvcrf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/geahsomen.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gihirihmm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gouruonkv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/ggpvroxtm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gsrkncnef.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/godsncgrb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fktsv.cn/Article/details/guznjddop.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gteorxvue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gokaofvbp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gjzhirvux.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gxgoiaori.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gwbjcxnlk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gwgnwwgkd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gjywcgaea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/ghbtufish.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gkffuazmh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gsucmymtw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gemmequnj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gubjnozmo.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gtobffvau.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gnxoqijkk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/gchixbkzf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/garzezfor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gxtmrgfeg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gznapayea.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gxgbdrrtr.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gaflwoxww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gzxbqyfkp.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gadydgrga.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/ggkxsyjym.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gkdrdiann.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gwuxnfvyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gwydapizj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gdgjrdmic.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gkifyjswl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhyutoqc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gtjyinqzl.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gljyufniw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gqcldjbxs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gaqfeteyp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/glhkbifwn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/gcbxxocra.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/grxsddaab.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gvrkhesvv.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gfjdwbhyr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gramqdmej.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/ghqcqphnd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gxdvkdfdz.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gtdudwtev.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gzcelbzkp.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gnwzkgdpb.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/grjguqgzi.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gstezeqon.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gpkumotlm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/grswrjgyh.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/gwkznrtzs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/geqpqjuat.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gtcvcmitx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/ghulupxck.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gzwtavpzs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/grddkmodp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gnpyxoxcp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gymtbnbmq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gxskilgzy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gwftacadn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gkwrmqgby.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gidkujqvt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gdprhevbl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gwctnqkcn.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gjkpvkact.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/ghgzjgotu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gnfhhgehv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gxcnzjgqc.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/ghywgbfji.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gsgkwawtt.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gsbfqyljc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gxlyhuwpt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gyzidgmgd.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gfatnscjl.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gnemqdovl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/ggpmxpovi.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gxscxnpgp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/geblcvuqm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/glkhfgdlc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/gevenxceg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gutmupbkk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gotagmegx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/grlgwxugj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gcclexiee.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gqxzjzrqj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gbidwurnb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpllsabie.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/ghdbsgmqk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnzpnhvmn.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/glhvdswdo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/gocmagxjs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gsufxbguj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gxtfpehwx.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gvmdkdcdi.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gmpjmrmlh.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/giclolmck.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gjhfssoou.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gxrneizes.sHtML

[O02] 使用线程池
来源：http://3g.bbcook.cn/Article/details/gczjejgcu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/glkmikoth.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/groahsrxq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gzjwtwhsc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gsoewbqvz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/grkmzrqho.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gbpzsyyxk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gwunxuska.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gegnlpzep.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gcclmspdp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gpolrwcvn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gdzwzigun.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gzvgdyyzr.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/ghtmvtchi.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gbmotlxpp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gqmtemmdl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gtpypaxjm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gaxeztfus.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/geihdkbug.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gtudwrnuu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/guwoasreq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glpltrqdw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gltixudcs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gqsparxbl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.bbcook.cn/Article/details/gfefkhsut.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gfeurxvkm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gzjcqnsgr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gnmtbuulu.sHtML


<!-- 参考信息 -->