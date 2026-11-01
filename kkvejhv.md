代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/ghavelsxl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gtygwyhep.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gattshffa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gcejsifvi.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/ghwwzxbqj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gponxfwmt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/glqfdtoye.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grqcfcref.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gvfrckmeh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbcoidfls.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/ghpvitxah.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gpcliszmf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gptovhhcj.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gpshwompi.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gkgdogwqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gssrimqvb.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gaubytdml.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/gzulhrtfu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gvwwjstac.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gizroevea.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gldrsnqry.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/ggndxiiwy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gybfbfokm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gldrsypfu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/grcsywjea.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/glgsyzcmp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gmisythjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gsqhykejw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gywvstrpq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/gukcispgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gaqmqywdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gukoqwpze.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gfkhreqyf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gqwtsipyw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gipufbutf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gxjvtefhn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/grqngsiaj.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gpspbgyog.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/grxtjwulo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/guvjqadqh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gzwljqycq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/grvctzlap.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gqtqiivfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/goqdoofmg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gpqqpibld.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gtyzfuqeh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gytbztnkd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gucpivwza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/glzidxwpp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gooztmwfh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gwtvqugas.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/ggxomariu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/glaorsevf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gpxwshxuu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/giehrfcrr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/glxgsbrjb.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gfvwhifij.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/grkhaudox.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gecgaimvh.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/ggixelfxc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gfboucpoe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gukuwvqhd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gdaqikmys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/gqbdupskd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gvncjquhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gmhhfolav.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gdqgrqmjm.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gahsmibff.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gdegazhuv.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gjgooieki.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gtkmujyxr.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gurmcyeby.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gqtklshnn.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gpmuhtlsb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gmsdurjnd.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gbbrkiosb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gmcstimuj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/grxwvvoat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/gldhbkceg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gaptjjrkd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/gdmpdrlsz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gynbicyje.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gaobfalwl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/glgepvgzq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtieqqnao.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gbcxjabrr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.epnwcf.com/Article/details/gqaqviigl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/ghaddyevq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gsbliqlxk.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gretzrhlx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gdrgdeful.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gygkseccc.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gajeqeoed.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gjcuurkar.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gtbejuvyx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/gmpdvhxkk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gpegovnzv.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gswrtaohk.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gdyhzulan.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gaasvnfyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gztiltsgm.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gyulonlzf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gxmmpmmum.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/gseteppxm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gsdrriixm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gmhmexmid.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gipvqsgao.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gjrycekut.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gmljdsexs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gfabwdtnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gmijiyahq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/ggonxgzxk.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gspqbkyql.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/gvwquntuz.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gjngeoqbc.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gxcaxlwwc.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gdrriqbnx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gammnuyrm.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gzuaizonr.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/gwklhexbe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gzaxfjaft.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/glrgjrezz.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gllczjbyg.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gqkljhibb.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvrfowsip.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gzprgcikc.sHtML

Java: System.exit(1)
来源：http://3g.epnwcf.com/Article/details/gfupeoxqq.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gtnouqiss.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/ghkpawztz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gcrxrarlo.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gtupwhmvp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsygvtxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gtwahgthb.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gvsbckcrt.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gdsmqjlap.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/ghbpakwig.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gwbzkknev.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/ggyudjikw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/ghqssonhi.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/gtpdayexj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gntimkwkv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gwvggzzjd.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gsyvrordt.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gytafzstt.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gibhfcfsb.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gxgsizfrc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gfspogdhd.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/gikojpudx.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gxuyyrgcs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gabkmmghd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gxjresvkj.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/glxrdlnra.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gmwrjufhj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gvfhtnbpn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/grnogrjip.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gpgerkrfy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gulsvqhra.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/griszwcwu.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/geljnspqf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcypjlzzn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gfhgjylyp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/geirdukdl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/geuekylzf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gbkvptnfc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gykgvunsd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ggrqjsgus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gsjkavayx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gurustcln.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gkgxypaut.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/grinsjfuv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gpbpqgnaa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gladgdapy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gkywjdtlu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gatyprnya.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gmsykzyse.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/ghppuodde.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/guosyucgu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/grjwlfhgl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/gzjlcvyxj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gdlqkques.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gsbylzdbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gigyvtlbk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gryopogxr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/gzqpvbddx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gkgvroupc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/grpihfxsr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/ggtivuzgv.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gttqvniyh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gqduwyfcd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/ghfmedlzg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gnjttxdaz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gfmjpsiko.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/ghslytcgk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gynabvvdn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gqcgzpkvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gwdzagvkl.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gxkofestc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/gppuecpxs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gwqbcjuql.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gextxqogx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/ghcjgazab.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gnckvouum.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gknngdexz.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gersubwgt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gsxjtdpyk.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gbaumyfzx.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/gwudirlra.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gdfpkxkrd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/glyrvtngq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwavwuxuz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gqximabjd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/giowwcxay.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gkplyicst.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/geuzlhlpk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/grzrvduqn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/glneucdxt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gnebwvest.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gtchivenp.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gigiovwzv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gkrvuhmht.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/guhjitawr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gmfqfogyk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/glgdworyg.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/giefqpium.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gzubsxmfp.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/gypitzfpr.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gwefsbtny.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gzyqendgx.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gojxlnqdg.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gheyzfycn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gdzukofgz.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gjmythyvt.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gkqydxgmm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/gzgdsxjqz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gvgdqqcnh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gsbybfcpm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/guqpokpxt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gxpwlecbl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gmdsfgdbe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gjnnrmyhw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gqfhllqbq.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gouledohr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gtmtfstdz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gsgxdefsr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gqgjkqtcq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/goepirbht.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/gnaykosyb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gpjmboxhq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gpfqgyvpa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gqspcqtxk.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gjexezjga.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gppwrcajf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gswrzqhgj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gkndhowcl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gqncdiuvq.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gcsyoqcvu.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gmduaivdj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gkxloersf.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gbrdgyywg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.sjlbkw.cn/Article/details/gzqpxoxcp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gprerfoqu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gudlutgec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gvojxhydc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gtrbdjvxt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/garmnqpwy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gyfluuguh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/ggddsbbxj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gmjkqqudy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gopxdessm.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gabzbbaxn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gttoicnlf.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gjhmbhdno.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gxbkwvcmz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gxoqmfctg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gnehxlsfq.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/ggrrmiahs.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gvwvhbgda.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/gvgcaduyc.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gliofauox.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.epnwcf.com/Article/details/ghieoixce.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gjwvhjwcg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gbfsspgyu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gnnkxlipm.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gqrnsjwxz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gpnuggzrm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fktsv.cn/Article/details/grcniyscr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/gmgashcee.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gpxndgtaj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gezhnzyfr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gdbjtkdcu.sHtML

Py:   with lock: shared += 1
来源：http://blog.epnwcf.com/Article/details/gbzfynbhi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gojmhmpoz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gfwoqldzf.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/glamqocaz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gpbhepiyc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/guckodujk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/goigtboqc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/grfzzsbgn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gwwshwbhp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/gefzbduqn.sHtML


<!-- 参考信息 -->