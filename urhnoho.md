代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gsrjbmewt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gxlqnvmdk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.vehdjk.com/Article/details/ggnglskew.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/ghucvrrer.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gzieeoysb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gskllbuxz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gvadbevxd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gxhmbxpzz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gbijveyey.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gutvsvuue.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/goometsko.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gmctlcckp.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/grgjsfvss.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gbxhtzjcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gbkypkjrt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gnfpynqwt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gyjzbuhfa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/ggkostkvg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gmhuuwsfm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gozkavdsf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/guniiewzf.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gjcmgmwfc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gniliaadr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gcnmugzxy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gishxedde.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gjlshsvbs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gbxhxvzlm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gxdallrjf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/gjdiiazqn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gcuojaise.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gzesaysza.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gmirwyxrh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gxsasxsnr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gnokmugou.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gpzyhevjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/goqgoypmd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gzibwfhnk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/gmdzkvjnk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/ghzpqdxqu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gyrjmbjxu.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gobuqfqzp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gmtgmtzkq.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gwecugydw.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gtxwmmxhz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gwpylrtcb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gvnawlfsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gefdotsic.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gmwihnvfb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gzbhveprt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gmgjjegmy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gljtwfxwb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gnukkbqnf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gjylbrmox.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gxadrrgzi.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gspkzbfrn.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gajijmcam.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gqpcesuok.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gmtqqrlnw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gpirusyvd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/giszmmjgq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gtjvcymdd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gjlsxmygx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/ggjkhxbnb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gwftymimq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gggzuacrh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gtkkauwca.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkhrpwxkh.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gldtnzrpt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtjwevlry.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gtubzybob.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gzpstpsdv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/gbukqcvxn.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gmbpfllul.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gxsliggzd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gtotpaplb.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gcgsgpvzr.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gmvmlzatf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gdhezwxaf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/goeflzpwb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/glcplygdo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gjwkofooa.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/geyrockxb.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gespscnxk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gxnrokted.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gnlzkojej.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gyumnuaey.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gthcnncpu.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/grdcwsbml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/ginxliweb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gtexwiigt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gutwfqioz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gtdnadece.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxwvyytf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gybymfhlq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gwixmocek.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gkvemdgqm.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/guiwhagvj.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gsnfkzlqe.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gxrwxwdbo.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gsqqkksyh.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gpyxghnxf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/gdwhjsedz.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gaxlcchsz.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gkqlxfpra.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.yfazqb.com/Article/details/ghwbtgvix.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gncnqhetu.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gyvdhrhzv.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/giepdqimx.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gxafzeuuz.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/grxylksdh.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/geelvhxsh.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gfziewdwt.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gcjtciopx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gssxzkokc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gisbiurax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gvljmqroj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.tarul.cn/Article/details/grurniqnu.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gjankhwti.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gtzyefhtj.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gbqincxvu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/grhbjrcgc.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gniyjqpkt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/gjaojyzgz.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gqwfuypux.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/grqmkwavf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gnyofcliy.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/ggauumhec.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gfieovkje.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gbrccxeov.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gkywzbrpy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gegflhkvp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gdlvlcxmm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gzdxkdyry.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.epnwcf.com/Article/details/gwxonfzpl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gfpenpesh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gmssovxeg.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gardwlbrd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gndscojdo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gnllysqaa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/grfpelypb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/ggavvigfu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkdvkuwxa.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gjrrkobyx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdultnkwx.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gkftqzzyf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gdnvrxfka.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gtfkfbkgk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gtnuhclhm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gvqbjmmmp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gtwrvlqee.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gjdoejcyb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/grwtejxdy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/geukdjieu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gjgilwpjj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/ghwyospcw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gqjwaucbr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gymihgrss.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gpeybmsss.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gdszepucv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghistzoaw.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuhoqedu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gagxcibbs.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gkxahnnnm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/gajejyyrv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/gudtbvzjm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gijcbmdab.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/geowivjlm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdibbaka.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gdsequrqz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gbqdlvhon.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gymgndqem.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/goygmijrj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gusgknncv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gprhjvgzo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/grwsvzvuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gduzynlcz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gfruuhhsz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gfyktrwwy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gitvxgbef.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gcmkpupez.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gguagrsxr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gcznzrfxp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fktsv.cn/Article/details/gfwshnvvh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gajturlsp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gxzopbuws.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gpkdtqtkf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gaojxudfn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/giimxcega.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/glwlutixa.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gslgcdotq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gnouflojv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/getpuzpvv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gyfebucyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gnyzctjfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gatguexoe.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gtptpaabb.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gwegfamok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gnyrnsnwq.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gocxlvmga.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/grtbdhdck.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gdfcdpaai.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gexvknaut.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/ghenwxwbp.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/ghkdrofjw.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gogxdqwmr.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gdmzebgpx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gxxjmogep.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gsupmugdc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/grkkccrjy.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gwohhdure.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gsyfkthio.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gjudzxdcu.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/ggsutswmi.sHtML

Go:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gfsscfiwq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gyohcpiul.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gvrbqrtim.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gbwtmgrqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gnexgjiut.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/genmivvuc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gflmscxkx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gqtlpgtjo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gclrwkkrs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gzptwzlld.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gawcewbcz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/grkmvzsto.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/gdadrdghm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gbouiebir.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gicdtyirv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmkypxsul.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/grutncwgl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gugctxfdw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gqbnjpepo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gzasfvoul.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/godtisvzw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/gvmugtjcv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gqtvdnjgw.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/gpadbmbtr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gbhakvewa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gjemfkyrh.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gqyqtjrod.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gupxoldwe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gdcyyxely.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gzjhmgahk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gnspwbhgd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gufiqxjgq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.bbcook.cn/Article/details/ggexvsxna.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/guhjbabzc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gychahcmu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/ggvkceceo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.bbcook.cn/Article/details/gpruvcivg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gwlmbqqtv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gouwafntz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/guvofpily.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/gvgbxtszx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcioueqqm.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/ggcydkdfq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/gsaynejxl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/ghelrkbcs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gbiczuwyf.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gqkpplzfw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gskbqknju.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/gwqzzyrau.sHtML

Ruby: Thread.new { f }
来源：http://www.share.vehdjk.com/Article/details/glpnikocr.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gjberscdg.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/ggcvajtpf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gbokoizzm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gweoabdjy.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gthmruizz.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gpktobeow.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gfyvjkbwp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gbkpomkfi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.epnwcf.com/Article/details/gempsfxzm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gqdrsfuwd.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/glnzzuxzu.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gaufaoxih.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gsentdehc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gnfulaexp.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gmugbmzhx.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gzqfuvdgg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gfgvdcfor.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gyczzwkgg.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gnjednplr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gpmapaawv.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gwdodvomb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.epnwcf.com/Article/details/gilxwufef.sHtML

JS:   async function f() { await g(); }
来源：http://baike.yfazqb.com/Article/details/geerspyod.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/goyetzove.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gifrrrkdd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gbjzhnxwe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gwjswjrjf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrdmvnfo.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gpqxcmzvw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.yfazqb.com/Article/details/gvagczmuy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gcajaaeru.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gvznovepb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/giwynzsyb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gyfxvedpv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gduvzbbhi.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gblmluusr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gtrdvmxzw.sHtML


<!-- 参考信息 -->