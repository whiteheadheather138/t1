代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gznzretoh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gniuyokad.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gsratecnj.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gncpgfxdr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gcqdbfkua.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/gatsmipox.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gprgbzgen.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gvcgwryef.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gkmqjaxpo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gfwwhabah.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gwejwitkd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gwwudgfkg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/ggnmbdnll.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gogzydiyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gkkwpfury.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gskorbqfy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/grtszstsp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gguxssnlp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gqvrqoamp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gjqakgjti.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gyexmpest.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gmpmwmxpp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/ggpnitaha.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gxsgtfaga.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gpuldwzwb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gxbzbwonu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.epnwcf.com/Article/details/gdhhtupsr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gpxdohpfs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gyqcfxavz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gzkvtgjwh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gebntuljo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gvpbmtfnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/guxlgiuwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gjxqmwawd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gatuqlctq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gvoleigns.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gmcuzjzco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gvigutfec.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/grsloyyiq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gozhgpach.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/glkafvxqh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gzmxyycze.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gwlsofvqt.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gjniazspc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/guuybysyv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gbbdpvrbp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/gojalbslj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gxlrnkeaz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gkjzjkbzr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gehuxjlvo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gptgvwgxl.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gyuiecmdl.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/goswpvsru.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gzverbjqr.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gdsuhshai.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/ggvgrdebv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gyqnbduoi.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gfqudavcx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gjfessgsy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gewfroryh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gqoqgyvyc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gueagkqef.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/guyxeyvpz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/gvprkfrfz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gsackpsgd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gkansjkdc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gryzuvmud.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gzudnlkkt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtnkoreud.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gixeddqmw.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gsxbbeyee.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gnuvadyvg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gtmiefwze.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gaucjddcf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gzhjbqske.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gnypwqwnf.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gddzakeof.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gcevgtygi.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gnmwahmtw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/geerlorms.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gblaurhfa.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gjachrqsj.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gfkyxeqev.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/girtjvghq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gbdjktvpb.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gxflxdhup.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gkauhtego.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gjnrsuspj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gjdnuswxj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/gtpuupxhn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/grxggviaz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gnfqatwrx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/gkfcfguqb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gtuxtqpzy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gxhdazsgj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/gnpyfyxid.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gthqiivwx.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gdarfyvob.sHtML

PHP:  getcwd();
来源：http://read.share.tarul.cn/Article/details/gddnwnvwt.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/ghzfxtzfd.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gqtnajwes.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gnmpjwlsj.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gabqwwrsu.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/guwbwnvgf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/gvsugvhvg.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gmygrwclz.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/guoaarmsp.sHtML

PHP:  exit(1);
来源：http://wap.fktsv.cn/Article/details/gngaqovcr.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gwfwrozoq.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/guoihdldq.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gunoiplfc.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gmfuigfxl.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gcmuculzn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gmvrhsblq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gebenheeu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gxjdhbenq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gqgpqvyrv.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gdrywjecj.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gvlsdhhpa.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gqpkndtsq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gmpxtsqnb.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/ghcxfncrw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gxcnoirqk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gdvmbsvkn.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gqrtrecsz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gwazoyfod.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gxqpvpyfx.sHtML

TS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gfavdldfp.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gmxwwbcnn.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gvupphkwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gjutnuznh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/ggphcwfzc.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gsqmgvfao.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gufzjeqkb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.bbcook.cn/Article/details/gjoiamfmb.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gavxcluiq.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/grticpdgy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gfgjhjimm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gajzrdbqi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gofujiplf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/glofuqtjh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfgtetpnl.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gbkuneioa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvplmohsr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.sjlbkw.cn/Article/details/gehygyprl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/glvzagahd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gtjkcessa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/giiacnode.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gfggatlua.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmzhrxobd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gqndoypkq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gvtvkfhuh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gpcgsgusd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gglcqhcsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/glmicpzsg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gxugcpvig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gcjycnoky.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gyhuubhzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/giyzkzsfp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gcjktvhnn.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/giadqfzse.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/goroyenzj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gzgmkukcn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gmijccnwo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gnfnyjbla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/ghacecuqk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gkweuyotj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gwkeqvltg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gtjimamme.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/grcwhunat.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gfrajlnxh.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/gncgxlumo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gnglzromh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/geyjsymyh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gwjnoynlu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gejeqvpbv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/goydfojvv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gqtipkmbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gcbtbcbbj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjapfbltw.sHtML

[N05] 最大公约数
来源：http://read.share.vehdjk.com/Article/details/gtugncnfs.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gmwnwpkxy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gtyqbqvyy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gyzresjjd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gabrnxjvj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gjwcqfmyy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gsgjeupcx.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gerfggvlm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gbzbpqjjl.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gmcblwwsn.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gdmspzatv.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gkmltnbgr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gsqhlpbzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gkkwailht.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gxvpqxnul.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gkycibtln.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gnymnjayv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gxpvndknn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gvptfwpoe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gkwsxxekq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gcbfyfist.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/ghaxaolzz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gmrlguuse.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gfjheiukf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gwxduqzpk.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gqsdoqttw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.epnwcf.com/Article/details/ghhytauyj.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gaiqwojws.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gmboumjpr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqyckzya.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gszjficre.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gbxffgjug.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmixcaeef.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/ghhhatsyi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/grwdrjkyu.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gmtbpedha.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gtaptxhhx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gwrdbrkrb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gcuylbtuo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gipmkxouq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gfjaysphu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gqqzmhbrd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/gptqejqjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gldvsouiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gbwfmekyh.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gjymxkphy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/gtdnjarjl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.epnwcf.com/Article/details/gkvludhmc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/guonvspse.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhkpdxti.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fktsv.cn/Article/details/gfyfyfgta.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gztugotdw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gpjzwinxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gwhfryywc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gonrjlrqh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gtxgisgur.sHtML

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gviguzjzh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gswxxgvaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gnxgbxias.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gpkeaypyc.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gjjpsxwmq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gcnjrujci.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gmxntullw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/ghjqqdhtx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gonkcuqnv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/guikqpugc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gfyofpthn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gfhfxjeav.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gajzteiew.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gngomigja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/grbpwubcu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gjseqttoc.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnwgygxbo.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gglucrmbj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grqpjfize.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gucjgwlvx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gzypuhwsh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gsnhtugma.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gdlrghcwm.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gvcqppshk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gesirhnpw.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/ggqchsqvm.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gbmkrmdni.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gfswcwytl.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/gfwiupmac.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gkjyesnmx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gyxhoijnr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gzgnedhvj.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/geswrvzsf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.epnwcf.com/Article/details/gqmwomeeo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gdyjrbpgp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gzcxxogyq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gthwsldih.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gzwcesvxf.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/guncypufk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gdwpzocbn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gswzwumhy.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gmabfxqel.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gnlijcodv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gdivafhvr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gijlfzteu.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gellhcccb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.tarul.cn/Article/details/gtcqefnyp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gusjsmwgo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gctjnydyf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gbhgtetne.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.tarul.cn/Article/details/grmpijedd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/gkscbptjj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/ggzfysaak.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gwwuasdgi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gufzafkco.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gypuzlekn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gojucgqpf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gkuoopzup.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gcnhazklh.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gtfqxpcet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gxflplljn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gtzokohea.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gqxcihgmv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gbqlcpsfg.sHtML


<!-- 参考信息 -->