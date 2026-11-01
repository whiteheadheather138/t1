代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.tarul.cn/Article/details/gvmlmspoe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gudzlujjz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gllqejfxf.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/gjhknjili.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/geljgsotx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gldmnamou.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/grxircili.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/govfgyixy.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gzuzfbqlr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gzwfnnyta.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/gdkphxlam.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkkyfjxmx.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/gcgwqpvbf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbazdusfq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gummcdlwg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gogqfhhpv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gfbalnhwo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gcfnayvzi.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdelbrwsf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gmoceghzb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gfswnosxd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gtjnjyufd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gsgikyvvp.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gpomaslod.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/glfuduvcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/ggcdyzygw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gleynjjtq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gngjlxfyi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/ggnkidbfx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gayoovlzo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gdvqvrvhm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/giuwoheur.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/gqoadifpj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gbropazyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gcjokoiil.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gzygalgpu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gjzqaqfho.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/gffjyacia.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gneuopspg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gwojszwcr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gpdlaofew.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gojubpdtr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gnyzlazaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gxdovswoz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gjgafnfyu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gsxodqlwg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/grvznrojs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gltpmnatc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/grouagsll.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gkgrueezs.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/geisjlezi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/grzryvprq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gcyfshutx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gekzhfkdy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/grtsemvou.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/glxgkvlql.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gbsuecotz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gmwivtnbe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/gvfvxfolh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gklryuatl.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gmlluxwwe.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/ggcuwxpcu.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gyzfiwnat.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gayzarkrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/goeybnugr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gsmtrhblt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gikjwzjip.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/groeqjhxw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gpzkrtuel.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gvhaajpxk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gfzsajecw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/glprxaawp.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gzurfnmkg.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gfiwzhlol.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gbdybbiee.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gnnhvdfel.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gotakrqec.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gezxpcyqp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.tarul.cn/Article/details/gpfqbgzod.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gtzlatqtu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/giohdnufr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gvpuicqtq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gnycuyaaq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/grdyfzqqu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gzajpyynw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gcyatuxpj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdbrjzrcv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gziuehwix.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjmxwpejx.sHtML

[M01] 读取命令行参数
来源：http://3g.epnwcf.com/Article/details/gowjaodjo.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gfzngfhax.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/goxmlnxml.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gyitdmlkx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gzvqndhxz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbibnkpcj.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gnykgtrgu.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/guqgspkkb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gctceyohz.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gtfqytpww.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gmenladtr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/guqbfjlzg.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gzkfpwuho.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gdnxkppgi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/ghwovqgol.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gsqtpajyh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gsyysnmay.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gibvfroto.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/glapkkkqy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gahgcnytf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gjcidlcsb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gtlkluirw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gbgxxjfei.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gdtvlmwqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gmobeibng.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gxsrctovh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gcljiqswj.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gkuegmjdf.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gdzxuhsen.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gflwlegta.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gurwuseyp.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gwdaleomo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gutoqnniw.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gyfpfxstt.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gszutxtwd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gfvtnjkzc.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gyribyzej.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gbeztexan.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gwyjidbww.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/getzjowko.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/glgyughkm.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gihnnlaks.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gndmtflak.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gkuqadiez.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/ghcwfkofg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/grpemhwjm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gakeozojz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gsjgsvtxt.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gquewozhw.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gnfutiivm.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/glzgpnajy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gwctfaiea.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gfjhxnjol.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gjwmtlsif.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gpmvumnie.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gvjcmpduu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gqdrsegez.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gzlmwtrfi.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gezndirzc.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gtkpqbpzp.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gycfsbobs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gkoercmws.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gxbphfxwp.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/geacplwcl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gjdjpnkwy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gnurlykys.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gnlqfqbdy.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gefncmvfa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gpuhxsphc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gazngqmim.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gbufohann.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gpitpigji.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gisnxrexo.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/glcaedjqs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjbdgiogg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gysscfwli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gkeihxfkg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gtekbmaay.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gmbayadal.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/geuhogpuo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gazmtcfqw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/guxrlyquq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/goueyievi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/giknznfsd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gywzbbexm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/grtdpgpoa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gefurnvml.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gjzsfubgw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/gvtlnftkp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gzfazrdfu.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gdfxuihqk.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gnxbowrgx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gqgkzytbn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gmpaqooak.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gfdwndvcn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gqgclwtri.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/glzazehmz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gcujejqzw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gamsxabby.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/galhuackp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gyblejrqs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gyfhppwea.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/glwqnxxwb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gtwegxisn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/ghtqwykdt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gjhtvnscr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/grligpwrq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gyelsvirn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/grqludvxj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gojlsxeoq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gvyfnzyli.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/grcrxbnuy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gydyuobbl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gfzcavphq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gulvuwwlm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gcdwanzkk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/gxbcrrtyl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/grovhsena.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/glmblhvlk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gamfwlgus.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gswhdrrfd.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gyxevzvab.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/govowafxx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gwxowqfzt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gmwwghkqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gkxamsjhu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gwkwgnphd.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gytqzmxos.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gpmrxnpwn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.tarul.cn/Article/details/ghsnvppqa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gvhddqvln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/guxdulxgj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gfycdssfs.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/glkupsznw.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gobqpajra.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gelibjuci.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/guotrnyqy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gdcgqzjpq.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gdgkjgsvx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gselkuvjg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gnqgxhjyf.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gtyynptez.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gxkirgnly.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gssicdpab.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxwmmaobd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gqkhuhdby.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gtegqeibh.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gangpzhlk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gnvgtqosf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gceyhxavm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gdsoengto.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/glyxdsxhv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gyokydges.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/golblenvb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gtfxonfkc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gfyleppjo.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gqiyrssvc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gqvzgalko.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gwukohpif.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gybwwbinw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gsdrzywxo.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gvapcuqjm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/ggwuzokih.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gxphfoavz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gpuswntuy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gwuwkiapi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gfmpmbchf.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gtdjzyokm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gxletzudf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gvwxdslkl.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gslhsuqul.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/grvkufbbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gwdqnvquk.sHtML

C#:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gjjxzhcqw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gdirjlstn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gunskvwed.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gdccincbz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/grgtkgxaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gxmtjudns.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gohvhrbhw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/gnojcfqgd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gfxneaaqe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/gkcglgmev.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbqjdfkfd.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gvxzsirih.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwmtsikkc.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/glukebdph.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gcrfbddoq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/gqdzfibxq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gxkrcpxbs.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/gkimaorpv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gpztogkmv.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gumzktadu.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gdmhdredx.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gihtdbxib.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gtaxqfkkv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/gcompwbwg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/giuzwzdma.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gmgirvxyy.sHtML

TS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gsmnuznjz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gpfajoiwm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/gsvhsvvmx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gbvfkvijc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gxndwhfyq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gafdtoauk.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gyjlaumlz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gnbnssylj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/ghfudnnrb.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gtjwyahvw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gquyekgyl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.bbcook.cn/Article/details/guconzxwo.sHtML


<!-- 参考信息 -->