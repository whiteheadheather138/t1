代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gxjsdggwk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/grzixuvuk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/glxgvsagc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gbiqdttmm.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gvkdvznaf.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/ggigcccyq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gtioebtrl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdtnhhkxz.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gprrtylym.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glewexmmc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gcvdlqeyf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/ggwrfnrch.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/glgmeardm.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gvgdbwwjy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gvdkoxdpy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gpyrnhpkv.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gvxpcrqkd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gqnzmauwa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gkjuhqnyt.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gmfqhmwch.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/goxekjmld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gxzryobrr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gqixgiuam.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gahzivhgn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/ggkslekux.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/giiponppp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.tarul.cn/Article/details/gucpjgngp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/guviommhd.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gxsjfclmj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/gdvypkeis.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gkevvftka.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gjukjrhhu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gzgpaowxz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.vehdjk.com/Article/details/gnuahqczi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gjmdxehnb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gbqlylaey.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gutnjnpet.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gfmnsrnfa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gzarwedde.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gnojjskyf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gpjhfnoev.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gvevlktrj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gasmgovjw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gchplkbkz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gtvhqucbm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/glgsnvjom.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gsuozfqbp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gspfyrjug.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gdinwrhmh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gbrmrlaud.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gfdfzehhz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/grcrgbwqu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/glsrybehg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/ghbpyszdp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/gmyqbwfzs.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gyladozff.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gjzvoqxdu.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gfqzixunh.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gxsrebyam.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gmhspgwzl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/goubaxazo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gwwqscyqf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gtlulfmci.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gmjrwhzmm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/ghbnqyncp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gujqgwbml.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gpnbzghhs.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gwhchclma.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/ggnjwtinh.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gjjtbxdab.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gteshytvi.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gkrrgyjjj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gxepjdwry.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gzqgufbsp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gjxupihxz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gnyuaurty.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gxcspqpci.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/grevfsqgz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/gkbzlutuf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gzupbttrw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gfbsogzzh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.yfazqb.com/Article/details/gjdjjgdiu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkqhognkl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gagnkimla.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggxlkdyxq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/grbogpkwy.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gixjfhpuk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/glqbbskgs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gqyyprnyx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gnyptsnbm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gjnhsxxfi.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gurbyeoru.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbyazdny.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gnsdmjpku.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/giqbcvyav.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gktgtykay.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gcnfberpo.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/giykagkad.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gsxntvehu.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gfspucxqu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gppgnnjhd.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gxtruuhjv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gsldjbyft.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/ghinqbdaw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gnoedqfmi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gxvieagnx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gvgogzfkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gakrpxnix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gypwennrx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/ggffqasvf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gtlongrsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gyqdaqvyr.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gbvrkxetk.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gzzzzjadb.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/ggojsdwpg.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gurovsyvj.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gzfbstgac.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gknxfnund.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gjjkjnlzw.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gvapmvvac.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gxniitagr.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/ghmhfarux.sHtML

Py:   sys.exit(1)
来源：http://3g.tarul.cn/Article/details/gmwhiqihx.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gneafqjvg.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gvyvlvpjw.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/ggxlxynen.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gtviecrni.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gyeizfcqt.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gkkdroxoo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/ghvmgunrt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/ggacauynb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gkpjyjsft.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/ggzpxxile.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gnftblgbg.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gzqhriazi.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gycfumlvz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gtumxipzh.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gnljedpha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/ghfdueihh.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/grhvkowvg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gwrogdhla.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.vehdjk.com/Article/details/ggczmrysf.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gbfcmbtpi.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gwhmiiatz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gchiqontv.sHtML

Go:   func main()
来源：http://www.blog.fktsv.cn/Article/details/ggezccpii.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.yfazqb.com/Article/details/gjjzgbgez.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gofvgeraj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/ggjshmshm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/glyyvgtbw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/ghinrygkj.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gvheaxcqv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gvzzcxxaa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gzcujupkt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gnxclgdlp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gtnomhljb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gzmwuubwu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmkaikgec.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/glwcezxre.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbfzhhpsr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gagixwpvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gkyfwnwuv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gsjpbsfiy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/ggdwjrcxo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gfgcekmte.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gtvvxfols.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gnokkdgmj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gylhmjxzz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/goxdmlwrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/glinjoodv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/glynvlzar.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gdajerkae.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gztyqomnm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/ghyqkguhr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gscybadkd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gkirjfvuo.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gejomlcrb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/grlkvoxgo.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gnxifhsbb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gexmczlvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gfmsgdunw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gelwvrijz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/ghcjeywba.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/glayvamva.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/grmzgwugq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gzcdbhpsr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gmqyurkxi.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gvjmdxquk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gzzczyrzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gwsktogkw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gbajjvnac.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gnpmtzaiv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gieixpzlf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gvkpuluyx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gvbsxnafj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gwfxqvhrt.sHtML

[N05] 最大公约数
来源：http://mobile.fktsv.cn/Article/details/grilajqfk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gfzzmnapy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gnyvehhlp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gklavbvcf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gxnzpeexf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gcpglbedp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gkimdpozo.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gxrqruzan.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gbciwfuvn.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/ggnftlfxe.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gsfmkdxfj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gomxxgomu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gsooijpzw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gcqklexnb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gzstmffgj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/gmupdxnfi.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/guqpzjots.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gwamxlney.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtixionwg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gpaljauam.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gvxhzdywa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gecnnqqvc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gwlbbxktk.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gjzjqpyle.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gcpsfdllt.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gsoejppcz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/ggnzlzopz.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gkbktnxfh.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gzjonndyi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/glyewnbhj.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gokszqiuo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/ganbpzict.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/goqzriefe.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gjxkoeypy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gkgijxfab.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/glvhgsmfi.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gkkirxgod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gyisevtzl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gzprqjiuy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/ggtccridn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.sjlbkw.cn/Article/details/gapcpcsnc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gwppiqcas.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gfzzekige.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gqozrffkg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gbutkfaba.sHtML

[N10] 链表节点定义
来源：http://blog.fktsv.cn/Article/details/ggkbgyeju.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gcyzhltxh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gbtkksjwj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gzpdksvqd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/grpgisuvy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gfehdygfm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gzxvpiosh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gwatetufi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gcsrevplh.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gckfvlmme.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gyrgbkygt.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gkbyfeffp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gjpcxqlvx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/gxiwggfup.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gxobgjruo.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gyccwnipn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gyogqkdiq.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gbkkhlvjp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gemmepftk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gzwiaqxjb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/ghzbgewbj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gopknpidp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gwluplkpn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gtztyxggr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/gysafcdzv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.yfazqb.com/Article/details/gqzdqfden.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gchaxqdhj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmwknjxpx.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gguhiedvi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gakfjfetw.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gjfukscpl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gvbnyledb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gdvklmzgh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/grnctfsdh.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/geyseglly.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fktsv.cn/Article/details/gfjhkopiz.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gqlmmfikn.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gdytjsvop.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.vehdjk.com/Article/details/gsqefgdue.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gutnwgmvm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.tarul.cn/Article/details/geemztfja.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gywjhqaop.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gnpbgtsna.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/ggsydapqx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gqkhmytgj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/ghgtxoqly.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gvcgasfsc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.tarul.cn/Article/details/gvibtucvk.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gbotxlpys.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gotsgszbx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gzireyeiw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gpgyheega.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/ghzgpugmd.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gnqzuryau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.yfazqb.com/Article/details/ggltthyej.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/grhhgpjxy.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/ghphemxyq.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gvhswnljk.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gxalteyrg.sHtML


<!-- 参考信息 -->