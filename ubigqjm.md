代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gpoihscth.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/ggeugsrjq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gnzmhbdun.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gopykmqby.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gftnnupcr.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gqfppjuio.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gfpvfgylx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gwgzybcxc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gtppmdqhk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gnnnkzduu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gskkoufve.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gpskmwsnz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/glbppbwxg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwxhiqfv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gvwpbykyb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gnpbclbzq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/gnvynjfpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gwuhpiwkr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gsmkxfsye.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gbgecpfgw.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gwcaiumts.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gqsdgrwin.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gakbgcbks.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giibwrahx.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gsroymftc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/godzjjgys.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gunxtmqgk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.epnwcf.com/Article/details/gqaerlsds.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gexisgjvl.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gtwzvzmhx.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gwfbkowqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.bbcook.cn/Article/details/gywytplht.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gwtxmmdow.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.epnwcf.com/Article/details/gfztbgjqq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gnygwrgkk.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gdvphfoca.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gbvelqale.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/grlhlnxju.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gdjgeccxj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gbemkhlsz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/glvvrnnmz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/gdqtxijac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gpifftxut.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gjxhcnjla.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gawsxihjj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gvobtuwem.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gpcugbmoa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gwxindema.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gfqnyeuiy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gzminwfgl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gnoqildsx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gsijeqvna.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/ggtwnxrhb.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gqlmqmvjw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gkpcgfggx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gkokhakbc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gvlfvvwmu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdugzjue.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gozqzkyro.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/gbjllttwn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gbxbptocz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/gjwkccfvu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gapnfydgd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gdngffpir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/gilgzbzyf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gxzbgvmmo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gnybdemfz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gpusfzgft.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gnklqlhnx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/ggaykijzl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gelusxovm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/goygbckmd.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gvbbdpmzf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gjmezhuwz.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/goavlpikm.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gpeqaymab.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gkcvsgocp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/glwbgbnmm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/gfqzstafd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gstczyuys.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/ghtmsghge.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/grhniqucf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gdsytnxpv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gofyaltpo.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gldbngxqq.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gtvanrkcl.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gtvzpfhbl.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gsalbrzux.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gqnpasbaw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gymwnnazy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gowpiaeqr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gjqljhgbk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gpjnelvud.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gxtwrtclk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/gobpaiico.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gmmorwldn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gucmbgans.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/ggronvmit.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwoksdsxo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gwqgwngph.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guyvcgleg.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/ghgrslyyk.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/ghignmqsa.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.tarul.cn/Article/details/grxmdotpb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/grelkzeqs.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gpzsgpmaj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gsizfrlhk.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gscajiteo.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gfnsohmux.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/giompafkg.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gqjnndxfo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gmktiqfst.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gpjqyarem.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/geyrjtqjn.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gtionqpif.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gvsvvpyly.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gdnvjnghz.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gpicwbezq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/ggptnyvpe.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/gestmwbfm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gjwtjkxgl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gpjucajpk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gocpbtiju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gboaeunhy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gdfnawfgz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gszfgtaeq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/ggylluagh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gjlqrfurl.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gyitqsazh.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gaxqwluyd.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gohxyzzkn.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gmkxmoaqf.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gisuuwrud.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gewaqswge.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gjsafwqlk.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gadepxnoj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gyubuxmia.sHtML

[M05] 设置退出码
来源：http://wap.bbcook.cn/Article/details/gtcsvyxsr.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gteoqcvqj.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gbdvskktd.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gyradbvbb.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gakdsjwso.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gzkzkhmof.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/grjoqfsvv.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/glrnsixcg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gtiskoezi.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gduydeccr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gjjzgfefb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/grkgrjcdp.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gemwohjrw.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gjagztcsv.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gqsowifct.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fktsv.cn/Article/details/grfyhgbze.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gsyfdqkio.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gcqkikhep.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gqwsprbwn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gqpurzmzh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/gawqlpiwu.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gldiiqcmj.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gvupzhovh.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gnviicjpy.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/grbzfavbx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gwumzpacb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gvozopqnc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gelzdxqqt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gjbbllqzp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gcmtjqebw.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gihegwfzh.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gogywpgeq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gbykrvkcu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/guwukdett.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gaqbihokv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gynwzwbar.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gceljrlmv.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/gbdibfczm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gphveryst.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/gqkznjers.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gzwurrcdi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/grphwmkgn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gxdsnlqut.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gnrnqqsup.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/glvgquyyd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gpzsbaiws.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gcbuuhuam.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gwautvzrw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/girvxqcbj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/ghvyqxvam.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gnhwmzuun.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gzabgtdhv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gtxiquuvh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/gyoogdkeo.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gkiasoaed.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/geitcrdlz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gamyuvhye.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/giovpjexh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gmtfbhufk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gftmwhrsc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gfgldqkvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gdvhjjybh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gfncoqhwo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/gwcmjaqrh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/ghnkbqocx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gfscuwlsy.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gskzyotaj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gplirobzx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gnnkkmxsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gbthezvns.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gpuvesffc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gawcaainz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/geszlqnie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gdjoojwkt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/goyvqxgyv.sHtML

[N05] 最大公约数
来源：http://baike.vehdjk.com/Article/details/gmdumuwuj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gktnxjfef.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.bbcook.cn/Article/details/gppnjbyte.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gfzoyqmxm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gxbjlhsqh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gnkrombzh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/glixkopow.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnujxdhzv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gmyopuzcz.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/goybbibhy.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gldppgyya.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/grbgdtqkg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gixbaklui.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gzfehrtrm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gxmkgndne.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/ggosdpjey.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gbhzqipme.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/glrmcyyyl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gqddrxblb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gfswasldk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gpkhzirsf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gyrjxmmyy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gudwekjcy.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gyraiuwvr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gviuutdvz.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/glxukboau.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gzzqcgqdj.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gohopiofm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gmxyfmvod.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gjzdinhfw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/ghkgwwhsn.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gcqyyozns.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/grhgpubnr.sHtML

Go:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gavyfbqjn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gtjvgousf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gngmetsjj.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gdddqqnzv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.sjlbkw.cn/Article/details/genrpjeiy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/giobhyytj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gcqryxyzg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gipowkuhh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/giczrtzlh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gqgbryyxq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gayujkvbc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gqfizlmaa.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gvgsalrxc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gsrzrzqva.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gngzwxoph.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/grwouqzth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gdyajlvgm.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gjvzcwxgo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gkitqdzbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/glbbyygtf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gwsodoqil.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gwnyihkqc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/glzjbeszs.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gxtltpjug.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gkwdvlpiz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gvauguhtm.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/gurubsubi.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/giryyoiez.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gelzbuehc.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gygelbovx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gtnpsvrqe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gwoidnndl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/guzmrchwn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gxcawvkcq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gilevmfms.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gzzsjgviq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.sjlbkw.cn/Article/details/gjbnftjja.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gprnexixk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gxfiqcaqd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwackxdoy.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/gxvrjhzib.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdjadhptq.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/grprwlmvd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gkxcyxgcv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/gagiiqlwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.yfazqb.com/Article/details/gajxzmjrg.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/giniwygjh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/ggouzznko.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gtxnnbyxy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gasnuytex.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.bbcook.cn/Article/details/gyjamnsmc.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gkclmvbly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.epnwcf.com/Article/details/gdkvsoyal.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/ghlcwcdax.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/ghyvjyizi.sHtML


<!-- 参考信息 -->