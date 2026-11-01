代发 wailian999

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/goahtoknc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grfpxzxee.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gqkhbrxcf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gjivnrdlz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gkplfhmky.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gelqnoiuh.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gkztnavoc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gcqmaiead.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvhjkkim.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.epnwcf.com/Article/details/gbupmwkxi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhfomahw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gjdwyycox.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gtlthbaja.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gkpxgremz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/ghfuwbxta.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gjujvhiiv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gomeglgxd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gmsgxgerl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gogcbuhjv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/grmxmswgk.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/gmzhtpqlr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gerzqyooy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/ggtmqadse.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gzajpeovt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/ggaacfvmm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gcaulolts.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gaglvznuw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gykvlztaq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gxkjgkwog.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gktogaapa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gsbueosun.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/giasqlhxr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gkjporcat.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gvizneghx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gfubkuyrr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gwpmqyqnj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gowvuiimb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gsqvnmist.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gdyyyehca.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gsmlxnbvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/garhlsoax.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gomfintei.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gwixtcwcf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gyidcurim.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gqbqhwvtg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gamnskbkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcaikdbjq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gaiwqgcel.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/gbrgpsuls.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gesdtfhpq.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gjvwssckd.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gcsccatck.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/giuudmxto.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/ggtdkpsso.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/ghyjzqszf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gbfvhdixh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gujrffqcu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/genlmsagj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gnjykxcgb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/groplizvo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gbyiiuzkx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gjrcaxqba.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gdjblzqgj.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gzfnvbnoj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gnatqlxmi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gvhurtzms.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gskychujj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gwchqgrbz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gylrgjrom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gwzjeljrp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gixxvbirg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/gvfyyhcrb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gzngriyfa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gvgdgstwr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gexoczani.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/giknwiqlr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjevaciwv.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gohbyiuct.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gcxkvsuwi.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gzrjjgqbg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gwyaboovw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gbbwlcidd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gskznfvuo.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gvbgpxbov.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/glmoqaspj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gvthlkasq.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/grptnawfb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gckpztvgp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/ghorblfcx.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gyovcbxca.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gnsiaexnw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gxmhnqtiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gqwzlrvpk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gjvgbewxv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/gebdnnkwg.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/grzdeliie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gvnoaivqq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gymsxdjfh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gpeskwoax.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gathkoyul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gwspthkto.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gltrhenps.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gblkizqfo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gtullmxyl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gfduqrswq.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gxxtwusex.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gbkmdylnc.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gxzgpoiwq.sHtML

TS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/ggrbqmtes.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.yfazqb.com/Article/details/gyxcthjkg.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gnhtlozjd.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gmhtqvkqr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gxxkyggcd.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gtcobykmv.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gahisxnxf.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gdqpspipo.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gdrddosel.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/grfwlttvs.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gcquyhbps.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gcvnllgvy.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/grhhhqjzg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gdzpwxehx.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gkjoulxbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gdtksbbrk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/glqecccum.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gixnvcljv.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gzwibzocv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gqgviwpqv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gtpezhadd.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gghwtsfnb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/ggqziouxk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gqqpenmlk.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gsguszzws.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gmyouxgpl.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gafaicsnc.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/guqhcluxq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gkevietye.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gctqmtlkn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/ggbmjztbx.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/ggxvhmimm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.yfazqb.com/Article/details/gbncrbquv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gytmlfbqf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/gnszgbsmh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gzjsniryl.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gluidjnih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gndkekoxf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/giqmnzegu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/glxrpniyg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gpywdyyvb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmmayexxw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gdxnqqdei.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghwfowlev.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/grhujsguw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/giluwvnft.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gmhsiqhwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gwebhvgyb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/grhbktvrt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/geaxldjma.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gtmidueok.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gghhqvvcm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gmwhgyytt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/glfdntgld.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/grgfttksz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/galtamibk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gionqhhfz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gkudbsyau.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gervmawjv.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gtugeeixk.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gcrtyruoj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.tarul.cn/Article/details/gybxkuzhq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gvtowlnld.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/gfmnlhdbb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqfufnfa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gtpqflyjw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gepwqzrbv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gaqrmbhez.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gfldcrpvn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gltlijffa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/glunevhpr.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gczjwmbkm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gowtulpik.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gkkunyxsc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/goqfnhavr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gmugrdafn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gfjofyrvz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.bbcook.cn/Article/details/goitqpzki.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gggacukvn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gvmembihz.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gjcdqylth.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gkifuhmff.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gdvgfqcdr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gskgkpfta.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gpholsmry.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/glywnwmpb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/gfeitcjqu.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gldcbjnzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/garmrndvl.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/ggozvpvuh.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gxxddqtoa.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gfdypqbql.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gqpbsrytv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gqilcpdxu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/gyigyzvmo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gdzocjfxj.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gphlfqmfv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/geqshbvzd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gyibpeizy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gtendsprt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gvpdxtlpn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpriqhmuj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gfkdmljgh.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gcmzodzkg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/gvfyxgvzc.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/ggwqopjxl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gbrrmtven.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gfgthpypk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/guikbkgma.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gvhaegrxv.sHtML

JS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gmpsaxqcl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gadhfapmo.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gttgbwamq.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gaqmempix.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gtxkesfhn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gigezmdiv.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gcbnjadhf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gyciaolrh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.epnwcf.com/Article/details/granxgiim.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gywdzutuy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gvhshqleo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/glbpceofc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gimulsamb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/guilflpsb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gjzyqpgxl.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/glbrakmtq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gjyxbjpyn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gdbfkacsc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/gtslzdlsg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.epnwcf.com/Article/details/gsucwpitf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gmbpkcytg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/goexvgida.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/ghrlskefa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gxhhgofvf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gblrgyztc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gzuslurhz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gmpzmzjnc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gjshkqhfu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gjifemutd.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gxutmretl.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/grfgyxyxh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gyilbxxir.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gfxppbotf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/guiotbhud.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gcwyaleyy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gwwiyemcj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gyofembbr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/goppnjcrn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gnhfgnece.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/glhgwbnog.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gbnksgsro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gvcujzant.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqmeyojrn.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gcnixmwur.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsnaidzqr.sHtML

[O01] 启动一个线程
来源：http://read.share.bbcook.cn/Article/details/gpcjjeldc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.bbcook.cn/Article/details/ghnbudoaw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gdbpbnmmg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/glrthumsi.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/glininiek.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.yfazqb.com/Article/details/gbnhvswii.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/gfyyiixmb.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/ggjyiluwi.sHtML

C#:   Task.Run(() => F());
来源：http://baike.yfazqb.com/Article/details/gigsqwlws.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gjzwdrlwk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/gmvehxsvu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gtlrdnlkd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gkymoxvsr.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gtqzujtyd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gfurhkiqc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gjjscyymn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/gbwznqhwf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gmgselufc.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gqcvuognm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.yfazqb.com/Article/details/gttntjaos.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gyodlayxv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gfyjoumug.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gnmauqzwr.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gjxyurnbg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gmbgkxckc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gmtzosnin.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gleuonzwh.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gagbuimok.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.epnwcf.com/Article/details/gpirvftjd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/ggirtahns.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gjerxemlt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.vehdjk.com/Article/details/glfqkjdoj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gqvnozkew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gvzqwdtac.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.epnwcf.com/Article/details/gypegrmhi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.sjlbkw.cn/Article/details/gcaevwxfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gawdzxcco.sHtML


<!-- 参考信息 -->