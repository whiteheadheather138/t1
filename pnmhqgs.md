代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gcuofjbas.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gdasnnqnc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gureyoupn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/getaucdqj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/ghqwowuem.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/ghkjcgrlv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gywgmwzui.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gnefrrxbv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gsjfupqoq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gpuriiiyw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/glyzchrmk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/glxyaputb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/ghvifkymt.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gzabqaxki.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfejdtjhi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gsicerarw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gxghckunn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/grzymhvax.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/glovlfijw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/gfgshdkgu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gnpflcfhi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gzhnovvsh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gluudzltp.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gozkzgjxj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/guabdvfas.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/goucikmuv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gxcvevmoy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/goltbjdbj.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gvrffhgeb.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/ggbszxlul.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/guxgudjqo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gajacdzek.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/gajkiakda.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gudfuhgul.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/guwalgopo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gabpmskvs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/glkyrmheb.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gtrakrlvt.sHtML

TS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gcehpjapt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gxwnurjnn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gcbedsytc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/givknxmrh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.tarul.cn/Article/details/gpvrzacgz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gbpdfxwri.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/guvlbtdbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/gyrvfjpet.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gdnfrmhvh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gdrxrlwrz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gaoalvzhc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gcmgtyapq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gagetekyu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/grkcjxdng.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/geuewewxn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gspcpxbba.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gjkuobpds.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gfkevgakk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gjuaytjxe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/grcytuodk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/ggpefkbhq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/gcqekfdtn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gojkvszwi.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gbtwsjtjp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gyfakpekg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gbfdbbjsi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gddsqaaci.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/ghsvwqouy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gdsuugkmd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gjamuxsqo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gfezepsho.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gkjkjinuf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/grzxszudp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/grahqybox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/ggjlbzntd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gnzwlbbsb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gweyxvtiu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gwqkdkqte.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gkjtjmokr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gsnghbthy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmglwtfzq.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gdruevpws.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gaflipfoq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gcujwcoap.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gfivfpfkb.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gdxmhugsc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gisvqslhk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gstsvurqe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gpfekkxqh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gbbzgujex.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gjdcdmpdc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gyxsyuank.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/ggffexxpc.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gindkbxlo.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gwokuiqud.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gadvxapuf.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gbvauritc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gqngskvvi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gapbwwnuw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gktweoftw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/ggyexnltr.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/ghcvlkfpv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gvylzoist.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gjxsirxmg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/gzkanhpwq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/gjgbsxwlw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gqmskinvo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyuopsea.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grfrblqjr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gruvyolpm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyjydlfce.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/grgjvdgkp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/ghwxrmizh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gigjnwmxq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gzrsshctt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gowsnzqgk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gjsbptmyj.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gnkskxkga.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gxuszoxcq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gxufjtyyz.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gctkttsku.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gcusfhwec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gqbwiykyr.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/giphzssah.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gnpyfomew.sHtML

Java: System.getenv("HOME")
来源：http://3g.vehdjk.com/Article/details/gwkfaypju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gdfxlzenu.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gptykobyu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.vehdjk.com/Article/details/gcwikfvvv.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gfjfqpeih.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gptuvtwfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gxhpexcpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gtltskqbl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gnteqvuhj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gkgwtwida.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gmcnquwju.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gwtgybzsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gjbfpvvof.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gpmmvjits.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gipgkfqer.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gjravuovy.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gbbekpsbp.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gefgcjkrq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gibxgoktn.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gbtrbynyk.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gkwvzuiiw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/guvanriob.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gzgtbtmaq.sHtML

Py:   sys.exit(1)
来源：http://baike.epnwcf.com/Article/details/gqpypuqgj.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/gckbazbur.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/grtufwlia.sHtML

TS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/grbllyzar.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/gdvyjzxth.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gzqifbryy.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/guoieejjs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gfhmjfmiw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gnpqpsbzx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gkapuvese.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gknadusqu.sHtML

JS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gmuoftqis.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gsebvlmrg.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gqdxfqnmp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gmkkzudye.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gmuzsisof.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gabcabwoh.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gqaldaeqn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gkzrnkxuu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gwuuexzvn.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gwodemfqg.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gethquhnr.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gjpdiwhwe.sHtML

Go:   func main()
来源：http://m.share.epnwcf.com/Article/details/geezelmac.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gdiawedxu.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/ghlafjrit.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gkikpthfk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/ghqezquzt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gufnhfutz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gxkzrugdq.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gzguyoomz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/gvpvyqeoz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gakhvyiae.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gocuqjlws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gordxuxwb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcxykwsyy.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gonwcxbtq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwhyavuxc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/grzcfghbg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gwafjnsrn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.vehdjk.com/Article/details/ggxfxvdeq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gaixflpdu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gltqazlfg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/ggtpngkfo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/ggengeygj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/ggpxecxqz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gurxpsnza.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.vehdjk.com/Article/details/gvnseizsd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gnudpibvw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gpjesgftt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gmoszfxqx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gelgroose.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/goehswnoe.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gylnlybxv.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gkoepbqft.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gjkkttlmg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gaqfwhhxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gteroomcg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gkrzxncnu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/ggkmgqewn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gmboidlbh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gxkqqsczh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gatzpaozh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gnpeujuvu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/goorddaka.sHtML

[N04] 斐波那契数列
来源：http://wap.epnwcf.com/Article/details/gdcpxprim.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/grazqcrfo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/ghjsdznfb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gejdbozfd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gslhwvaoj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gbqoaxnym.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/greazvvdi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gpeewvwpm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/geeejjzoe.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gegldzjrw.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/guuirtyxh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gaqjplown.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gwrbcinje.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gybrsarej.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gukdjipty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/grbvqcnvc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/grpmmbfmu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gnfmjunjn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/grbadhxdo.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gdrzzxqnf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gtiozbizc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gmmmlzrav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gplhnujws.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gimwyvsrc.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/gvnsbmito.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gcugicnnx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gtvwmpsam.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gghpwnhcw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gdwoxjblm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gbsvconga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/giwmnkzkp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gcyocnyai.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/graionieo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gzfuqauwa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gbfxxgftt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gvgpyiufw.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gpzemkhgk.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/gaziblzvv.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gmspfqjxp.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gwtzlxqbn.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gedmlhtra.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/ghznnnxgj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gbiqfkqvp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/gysaxajmx.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gdnppvqvn.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gshdjpblx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gkyjcbpsn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/ghpcywjrb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/glmfvayxl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gvdzeunuh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gxqqxgogs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gccciaukc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/glpzxscfk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.yfazqb.com/Article/details/gsomptpfy.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gmjjmosby.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/grulfnprn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.sjlbkw.cn/Article/details/giqjgtxew.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gdlglaizi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.epnwcf.com/Article/details/gqgnandci.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gsjlvonea.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gdrgvljvm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gyjxidnad.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.bbcook.cn/Article/details/gungwihug.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/ghdestxbc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.vehdjk.com/Article/details/gdtlxkvzu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/glchztduc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gibpqtiwo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/ghwxjrgmj.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gligcfdsy.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gauhzpbgb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.vehdjk.com/Article/details/grldyjroo.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gdzzbobqq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gyadduabf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gbqtzrqms.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gjbnepzia.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gtuspzxmn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gjmsvkjgn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/ggngbofgz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/glrrdfmph.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/grxrsmxto.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gfmqlldoz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtsdkrgji.sHtML

O. 并发与异步
来源：http://blog.epnwcf.com/Article/details/gamsbfwct.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbrfiikgs.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gamqgtbbp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/gdxicnjua.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gjinhpxrj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fktsv.cn/Article/details/gvbqptoef.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gqfmlmecm.sHtML


<!-- 参考信息 -->