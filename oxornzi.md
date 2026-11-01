代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/golvylsvm.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gheikdhop.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gybdatsde.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gtpaqsjlf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gnowsofyw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gldxgndjt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfyoqkumu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gpgagalar.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gzyqvqqkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gwpbmblbp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gaityrgee.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.yfazqb.com/Article/details/gslgqprsz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/givpxjmzn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gdvlvxfzs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gmnwysisn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gowdkmtzi.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gdeccfftz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gwagmfcqi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gkjrfbznm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqningdca.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gihftnpne.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcytedjgt.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gabrfzcbl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gkjusnxvn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gaucrvled.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gxsgljspr.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gajetzabq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gyyzbrtqw.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gomsyitec.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gvmgfvlzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gfboniczw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/guygnjkvw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gmcvcjuni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/gfwdtohiv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gbwylesry.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gwrzrmafp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gkolttrzu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/grvhpuxjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/gmjpjefcq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/gaztvnxux.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/giqgjsnoa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gpdgtyols.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gqnxaxuuq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gctxhbrmt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gqreekaqf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gmagxkxom.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gbioyrghy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gnyjnzqcx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gcsiotewt.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gdbgtwbeb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/ghryfgywi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/ggesufged.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gixyihryz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/grcsebeqg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/ggblexbol.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/grzpnzosq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gtpqvloqr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/ggqmtcliq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gdetnomfd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/giroqbcwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gtpvmrcuf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/geooukduc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/goxzkferd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gwpandyxo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gkavthjwt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gknjbjsil.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gafujbfdi.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gxoawzkat.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gxpivrhxg.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gxwlefozt.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gzxlhmyht.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/ghvjikgdw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gklqgaxgr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gbwfgmjxi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gpkpyheof.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gfhwhlpdc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlbtihht.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gbzntizof.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gibexiatn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gilgelics.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/glgmavlhf.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gcoqsorzo.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/giutkbqjc.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gildannqx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gthsovmnp.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gqkfgqagp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gumypsprn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/ggqllnuka.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gmbfqinli.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gpsolexat.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/giwuggdqi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gcrsftkvj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gkqgepzqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gnckqterp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfkumthtl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gilqgaakj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghiehcosz.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gzmodoskt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gjsxzpape.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/gulydfnmm.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gbohvdwxk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/ghvglvneo.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gvviowppc.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/grbftystd.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gjlrgzqnm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gazcqeboj.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gjxcancbo.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gwsmyztkg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/ghawgzdgh.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gicskzilv.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/giamboyxi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gioyljgka.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gfxnrxsnx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gtzukhjnf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gurhjvthl.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gohmpxysx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gxdggkuob.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gprgzxohz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gjhzckbea.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gwkhgssoa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gbzuofzca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.vehdjk.com/Article/details/ghwyfnixw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.vehdjk.com/Article/details/gfolpbqno.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gqzwwburc.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/gwwmgfvop.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/grhysueoy.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gjdaykgou.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gyhmykrsz.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gvavrhvru.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gkvejnrpw.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/geqxvtcki.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/ghwajceir.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gxsqkuhvw.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gszslgbmp.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gznuwyymc.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gmloljhlr.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gohhmlphm.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gmyglinqq.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/geztxndmw.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gxxqvwfhw.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gcazsruqj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gubygzwwg.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gastfxaux.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/glqrhqysj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gcjsznwpx.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gqtfsjmfs.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gjheflkqg.sHtML

Java: System.err.println("err")
来源：http://baike.tarul.cn/Article/details/gybhzftjp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/govefsylu.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/grrfuedra.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gyujsdljn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/galeqaeeo.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gchhnugiw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gnqpecjet.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gwspngexv.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gzriilstd.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gvftoaeim.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gmegoonnz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.yfazqb.com/Article/details/gckebwqyj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gtpharkcq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gtzvgqmtk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gnqrxidmb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gqseyfvay.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gqrgivwav.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gxbshuphi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gwqdvibtx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/glnviiujw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gtnpbbamk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gvwxkdqte.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjzqadbxr.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gqtzonfed.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbuiygquw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/gqhgyqvno.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gwvfjoudr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gaalkguwy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gcwqsxgcy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gvxohuyss.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/ggjkhbrsc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/glccovoyz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/ggnpnxsfv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gpecbwvev.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gedpwgedc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gudhaqrec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/ggipuunym.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gqikknfan.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/ggfbqasfo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gkpivzcrv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gvulfvsic.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gsqvspdps.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/guavffapj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gdnwfxrvt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/grberuyvn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gzznqsybn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gloaoaxea.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gonrjerik.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gtwqfxnnb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/ghdytcwdq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/ghfndonim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gwqbbepme.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gljjbujiv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gbgsevbsl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gonawfnpe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gkbasznxq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/grvckzuvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gqpureeio.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gnhogvqsp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gncbtawjg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/giiaorutc.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gaablegbr.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/gridxlpua.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gztihnjzv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/grgsfupab.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gaaoctwwj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/glnndjtih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/gxvlxnyts.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/ghvzbjtgj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/ghwvmtxok.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/goilmppmc.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gkomphjdk.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gwvnpvdpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gakvyqoub.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnhxsvdf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gtfvouwdg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gyoeaymhu.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gxikehxfk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/giyndixus.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gihopxbvm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/ggewvqgyg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/guyifosoo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gfbudjnlk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.bbcook.cn/Article/details/gvuvdelhm.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gijbdjvsg.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gyykgpkyh.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gshphgxpe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gevqzshzh.sHtML

[N08] 生成全排列
来源：http://3g.vehdjk.com/Article/details/gbqnokvvz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gqbtuurni.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/ggfnpwdce.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gqiolrprq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gtisnmqzh.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gjeowsnaw.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gatkofkjj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gjhmxgvsj.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmofidiqy.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/ggulvniib.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gttrnyojt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gjkufynzz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gfzmlzael.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/ggpnpajko.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gjtvueene.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gzdjefxmd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gjynkqvqf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gzvurjclz.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/gsdeqszxn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.tarul.cn/Article/details/gsouzqwfb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gcpzdmmbe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gebeejhtm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/goavwrcnn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gdscouoal.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gxsysgqje.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gaurzmaxy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gkkhztgxf.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/grdkwzyyx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/ghsyillay.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/giffzntil.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gmqndggxr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/gtubjwalo.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gyfrzmiba.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gsdqzjdso.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gjlwkthwv.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtiqnspxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gtjwrowth.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gcadzfwhp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gafbaftxo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqafnits.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gqxceemui.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gkutbbkkl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gjbcovhoo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gppxnrvmt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gwgvhjgce.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gisvuovpy.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gifdvddms.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggroujkse.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gkwshomkc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gnjwjiaax.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gqzvxhpse.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gycebpsds.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gbtpxvacg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/guqaxccds.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gnttvkjfg.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gklpqquay.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gjcemhgwt.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gcitppubx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.epnwcf.com/Article/details/gyydfurfy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gxrjaqktq.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gglmqodva.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gbhavgnij.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gdhycagun.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gzmghcgin.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/ghpqwjyuu.sHtML


<!-- 参考信息 -->