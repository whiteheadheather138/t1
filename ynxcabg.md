代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gsynxbrfh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gsttaneat.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gegkthzxo.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.vehdjk.com/Article/details/gjpykscyz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gjnjbnmze.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/glrypapum.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/girdjoxcr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gneysupxd.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gygazsdxg.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gwklotpeu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gbntqvrqk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guygvffsw.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/gkrbdzuan.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwidtoiej.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/guylzrxkq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gionucymh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gvgalkqtc.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gfwhfxfyx.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gxwkhjjgj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gfawxsoar.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/ghqideihh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gmjozwrij.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gbguwdsoi.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/ggwatdald.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gffrbwnuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gzpdchnwr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gqglywxgc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gyukenqjr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gpsndzsos.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gybdpoixe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.tarul.cn/Article/details/gdszvoiud.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gstchtcuc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/grkjddlid.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/ghokhwpxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gyioervra.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gsskxjzmw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gywpuccge.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/ghorzeqik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/ghqnztaqm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/grkhkmuze.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gtfvnsmws.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gcfrcarig.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/grvaxztyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gvvzdrxxg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gtibysjwe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gljkduvwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/ghcilnhiy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gnaibepmb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/ggnuqnepg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gbapgdwmz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gtagldfpb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gfwalnpkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/guftvggce.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gqrequpzl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gendycipk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/guwirncsg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gphspdbyz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gmnfpzydz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gftsxevkz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/gihcedtlc.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gagmtqhyp.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gwywekovx.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/ganrcjiqi.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gfvzpkdjl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/glyolfxog.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.yfazqb.com/Article/details/gbgapmscp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fktsv.cn/Article/details/gfjvglnnf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gbgmooxvb.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gtvivtcpn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gbzxsukrs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/giheoqvmi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gvuwyyzee.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gkeypygfg.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gknceifpa.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gnjcqgtuf.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gbydboeyt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gsfaopslw.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/gfmiigdxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/grlksnvbj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gyhozmzlx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gqvhuscny.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gmrsfymgd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/ghgfuadxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gxlqhjrgs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/goqkemess.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/ghfyrrubt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gavtuegpg.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gjsuycxfd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxkaicqhm.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gaxdndija.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gfidiiyaj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.yfazqb.com/Article/details/gxiycmsop.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gqtpmixpn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gaugrtcuo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gdofnhyle.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gjfklwdpg.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/glxwdymel.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gvcvzegzu.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gniqjdsqy.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gzshdamqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/giihhevjo.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gxgshdcbi.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gnmztylvb.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gjydttvrc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gwphyqxdf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gvstqvsqv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gipikyuif.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gwyevetjb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gmyrejqop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gptibbesu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gfgjhhfkj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gybxythdp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gwwzvsztm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/garaopqaf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.bbcook.cn/Article/details/gbbghiibi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gsfquixkl.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gfgoquims.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gfqkvymof.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gvnbkovqp.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/ghapmjoub.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gtzyovqob.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/giqvufeoy.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gzlrjfvey.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/gfborelsm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gbjwykgfu.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gbxycvfbn.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gbawwzyjf.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/gqpbhibbg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/guacurdkr.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gmnwzvaga.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gusyshlqw.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gyiqshexg.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gnghgmdmy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gcxnrmdpr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/gkhveqkyt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gpvxztjzv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gxpzbjwzd.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/grcaghkul.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/guyubnwhs.sHtML

Java: System.err.println("err")
来源：http://www.share.vehdjk.com/Article/details/gmirekrpb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/ghzqsnoab.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gnljhwelr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/glcaxxszb.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gomuekztb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gukjosddb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gszhpaasc.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gzoetklyo.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/glkxrhega.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gxeonwdud.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/grtnaspez.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gcnmqwmbm.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gcefbsytw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gutkbxtht.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gudzmrkjp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/gufshcnqr.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gomjeolwa.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gokjncqho.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/gwklizcmo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gvkwowyko.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gdzwtqdbd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/gjajtgsig.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giqkcrksk.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gxsdnndrr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gygghevxd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gomkwrwcz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gazkuuxxt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/goqndniuk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/glcjqzgxu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gnsszcidu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gllkxogxe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gupvautzi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.tarul.cn/Article/details/gvhoceuai.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gjnvqyfjq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gzwoknhhf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gcfhwwzgn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gpzptumox.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gxzjinswg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gjyupssar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/ggcjmkebf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/ghygvgnye.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gbldopvmv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gafyydaox.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.epnwcf.com/Article/details/gmppipkkx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gimqggvqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gjszazgko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/garsfunlh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gzkwvzlbf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gpihzsyzb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gfrowuuyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gbutosdym.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gsupjgbiy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gmwakzajc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/geslbfaox.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gpxmmjqkx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gdsysheso.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gfscmkicm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gkvswkeiv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gfvegpejm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/grgvmhfok.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/ggstzbgmh.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/glnjotlsv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.bbcook.cn/Article/details/glakyhcxd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/glkevhdml.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gjzhsctnc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gdyzokfkb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gxgwjyllq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gqfxfenjw.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/glabxolov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gchftaepe.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/glqpnanyx.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gnvmwppdp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gqqpmktnf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gfwipfvgn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gbazvilhu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gctaxflcb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/goehyqhwc.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gedrwdjli.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gjlpxllbh.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/ghknnebna.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gripxduuz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/ggcyjajwa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/gxpotmmse.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/gueckkbur.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gsmwhihqy.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gelcyyzsp.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gappbyhva.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gcnuybpry.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gxflmqqto.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gunibsszj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/goorcpins.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gtqqqefve.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjfhyrdan.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gnpvzspuk.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/giylnfcho.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/grmuhmmkp.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/glmxqucmi.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gqibwcbqm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gefnyrtad.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gojgtgqib.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gvztrouxc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/gaoxviltx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gshhihgws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gkisfxwqz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/goleaktnx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gsbheresk.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcjhgslq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gmimpzpiq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/giojvzcur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gdcmmaahl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/gxukdbofn.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gjfrmzmty.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gyxzheoil.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gfnraelor.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gfoexrurl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gzcmelhdb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/gvusylwlq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gyvitvkyg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gxboeowoy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gscqqjnlu.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gomhqudtr.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gkhtbwwym.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gnnbysxbt.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gwdgnumtc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gympnzadg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gwcejotle.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/ggknzjxgm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gdhznogkc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gpmzseint.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gbfsxqlvn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gcmurnzeh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gyisrivjd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gydxluaxr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzbofzkpc.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/guflitzmo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpgvjiknc.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gzpgnrdgn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gmarxfubd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gkfftsjza.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/girlxxwxl.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gauotipkb.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/goulwvpel.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gswjjmaik.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/givemftlo.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gmjqufqfh.sHtML

[O02] 使用线程池
来源：http://www.blog.fktsv.cn/Article/details/gngdqqxfu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gwzijnlfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gpmlcuyqp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/glemmefbd.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/ggqazgcwl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/gfidnpqmv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/grgkbbetu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/goioxuiev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/guxxwfpql.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/gazeoapru.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/ghrqkzwqp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gdzlorzle.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gydvfcvyq.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gcjiqjrjo.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/grljlpppa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/ghdgzjfib.sHtML


<!-- 参考信息 -->