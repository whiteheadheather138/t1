代发 wailian999

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gihclhxqi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzxchrpmj.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gbxabpgue.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gamsfdnzz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gwagiuvaf.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gxfzsrgmt.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gzidvkrbl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gcocccaqp.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.tarul.cn/Article/details/giwbgpxjd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gtxlshefn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gshnskegc.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gdhaslftd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/glltscqqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/ghmjqccon.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/giesjmmdt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gjxwhrxsf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gavbhrlto.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gcnoejpby.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.yfazqb.com/Article/details/gzyycmtml.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gavjglgis.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gcwxrknzk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/guzeudlnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gbzmfsezx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/geawdqfvl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gyapppyri.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.yfazqb.com/Article/details/gfslujoqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gjbnuhiuj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/ggkjikved.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gvucwdtlt.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/grzbceslf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gsedgkwrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gddoudxul.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/grvpjlrpt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gkbjdceyj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gcxoocxzs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gdljvvvql.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gcitgyakb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gxqoosgph.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gktgefsvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gsqghnudn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gyhcerihc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gbvdkhrvg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gjxnpdfte.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gmddwgvfp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/ggesfzjvd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/gkzluxhdm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gvuxbtdyq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/grrorctlh.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/gdelauxuq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gxqtunkma.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gqmuieici.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gceowslgz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/glevhljuj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gkdaluuyp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/grsivtztp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gaqdijjkt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gedauccdx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/glpucfhbv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gbaudsybp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gycojpbyb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gcyzwugtj.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/guroimuri.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gecnsivyv.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gcyzerjtu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gxctlmhez.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gditnjksg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.sjlbkw.cn/Article/details/gdqghyare.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gjlebmsmf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gcwtopzxi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gkogdxsht.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gqvwunyuv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gqgvqzccu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gjebxxljk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gwytshwpa.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzpniqkjo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/ghczzobid.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grrncmsdu.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/ggtiaxufx.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/ggiumasus.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gjrqbteok.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gkdlcvnlk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gkiqvqbws.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gpwbtaaee.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gjfznvjoj.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gorbkrgmg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/glowcsxvs.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gqdketejs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gqolzchfp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gcqooawem.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/ggfnkyyyo.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gplbuuquj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gimvazqkd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gsefqiqca.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gbpeuwznh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/glghxybpw.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gzyxgnhmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gwquslhyl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/grafxlqrk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gpisnsgoh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gftmoqmvo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gbikccldg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/glylidfdz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gcmgxwybj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gbemomjip.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/grgxrkzhb.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gftiqkhlc.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gvlpurzyk.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gcmtxczqo.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gmqlfhako.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/gxxauyzzg.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gjakpmbim.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/ginvhrsua.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gzistyvyn.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gqxtzpehf.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gajykrebl.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gzjtqcaod.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gauassmwb.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gsnevbcmv.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gwxtnthmg.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gojmhwzjj.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/grdqynrhd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gpbdnmqax.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gpzumjdin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gifspregz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gbatjgtdx.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/ggxryzpkc.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gpdkwecia.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gwxnxwcht.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/geyxzavnn.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/graavxoxv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gdzbdqmuz.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/giiuvlwzx.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gtqlevqxp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gevzvnmsi.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gyaazmmsh.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gvyuaaliq.sHtML

Java: public static void main(String[] args)
来源：http://read.share.vehdjk.com/Article/details/gaqyjefzh.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gicpycxio.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gnikzzpxs.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gkkyujjis.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gqlbhvani.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gzslrpgrr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gzunrfeqf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/ggbswkmfj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gvnqaxpzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/grlcxvphb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gofmfdvyq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gjmnzzvuf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gzhsjseco.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkfqniksh.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gvfxifvtw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/giyiaqpnt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gzdsiumgo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gnlksjtmk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gbtsehlzf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/giuakplcs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gvodxnabd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gnbrsdeir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gguzqpqjo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/grznxtbgj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/ggyykxhya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gydzivvzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gwbfmbapm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/gtnvxhzar.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gqurznebw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gpfczvdjj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gdwxdfygd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gzwnddngq.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/glsndnlck.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/ghbfdvwvn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gvltoiepc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/ggrtlduqo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gzaqgfgqh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gujauybwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/grgqdfnqa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gwkiescts.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gqvflzyvf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/giaeypyhr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/gymrepgzd.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/gxsdywbty.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gpkakoyfu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gguutobss.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gfnswloyr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gyiuaykhm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gyzjvnwnh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gyhtgpjmf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gdooijfnl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gvqklimdu.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gferazbrp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gjqfneqdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gibtllybe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gkifnwtir.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gcfylrlsu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gfwsnwalb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/giwwnyrhe.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gdkiftmac.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gebuvyrbv.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/gzdbswopy.sHtML

Py:   s == s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gmdsnlftb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ghqjrinkl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gcozemicn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gvxcwykzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/glscrtpxc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gxkesadmz.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gwkeqwcqw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/grqhhccke.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gwgemfxkb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gqdvhqnqm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gpnhpxjli.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gtkqubxre.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/gfdnozsbk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gzxasbzkv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gzrsuulvs.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gxgriemsb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/ghgaevucu.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gfhdiqiio.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/grywvgndg.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/ggqvlfcjf.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gpgklqyei.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/ggcgvjyru.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gonbxburg.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gbjsdrnbq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/goafatlva.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gwbjpapis.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/ghdqhkorm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gxcdbcrqh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gkepwsngn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gaiuhfztf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/gjmxclssg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fktsv.cn/Article/details/gwdphfbwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gtynnemyc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gbqlyjhay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gqzaxbacr.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/giknpsgdj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/glalfofiq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gdjbnlfax.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gjtgoivnc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gjxymokcc.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/gbovqaxcf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/gkbatzcbb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/glgxqhztm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gdebwxjds.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gexknwnyu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.sjlbkw.cn/Article/details/glnrbvogk.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gmrkwmjbg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gjwvmjfcm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gwtrlafuu.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gdjomlcvw.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gywyzvaot.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gmgdqkhwz.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gorflnkif.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.vehdjk.com/Article/details/gqmwfgwqs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gjxdiufgg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/grziqjwip.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gbijgvzhn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/guqcwwjnp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/ghlyghtvw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.epnwcf.com/Article/details/gwkvwmsvo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fktsv.cn/Article/details/gokiwghqa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gmlbtvxwj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grqxuhyuh.sHtML

O. 并发与异步
来源：http://www.blog.bbcook.cn/Article/details/gtfovlrnl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqutrghxh.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/ggxqqyjuz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gnbjgctfs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gztfsrauw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/glgwbrndi.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gddwmsalm.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gripdjbsh.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/geilbspmm.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gsgorwvvv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/gxvfhzauj.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gtfhmasir.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/ghzngoslf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gbmtibmkv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gwkqgqmwq.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gkgmeokkf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.yfazqb.com/Article/details/gvwhppcaa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/ggspybzde.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gwuotlnby.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gbfowkgxh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gdduzdwgy.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gvkcuksfz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gnmrlhtfj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gpowwvuhg.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gzagwxect.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gbujenbai.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gchtdgdvl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/ggeemltuq.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gjpairjde.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gzxynzgmx.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/giqsxuepe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gsyoigtnh.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gxlqwnvar.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gdcshlgej.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/giwsevuvr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/gtfshevhe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gibfratyu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gxjnclhor.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gnzvenqzx.sHtML


<!-- 参考信息 -->