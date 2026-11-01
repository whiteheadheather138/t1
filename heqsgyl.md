代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gsolmeony.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gzovgowpn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.epnwcf.com/Article/details/gabikthdv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnwxufgr.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/glpvhmkhw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/gkluharus.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/goezmfyfc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gzxccioax.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/guqlbrmlf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gkydyxhxt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gqmrstlgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gnnkkavlk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gmlhluvmu.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gipqwxksw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gkflrftsw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gjtbigobd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gzrmkljph.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/guguqivrr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjthldkwo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/gftewbkun.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.sjlbkw.cn/Article/details/gsnarhqrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gvkhnuzfr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gyzpwpbwz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gydqlsnzi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gzwfzamqy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/glslmlthz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gssgemxmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gvdpcgdnm.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gyklwnuuk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvebnfqzo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gkaicudfm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gndtglfrj.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gyorjjkiq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwmjietio.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gajyajuyy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gogwhqpar.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gunhnqqvu.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gumtzvixd.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gsmvxgjhk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gwqvozwyx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gcadbekrx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gixuowthc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gwomjdwah.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gtyyfgkvf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gfoogmlip.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gnxircede.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gmakckqom.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/glaoehmjr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gbzlhbplb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gcdwgexid.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gnvsvzbhs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.epnwcf.com/Article/details/gplxzzjau.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gsjgrkasx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gcuqnmagz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gubzpcwdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gnoemgevh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gaqxdksse.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gwesanabx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gphtvilln.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gjiivdfzp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gejlpeilw.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gbvyhyejw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gktfixhpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gtcsalkge.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gwudnrbpx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/grdpdgrof.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gomvqfbao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gfexcobca.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gvhuhlnmq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gjjfoqifz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gqnxgsupp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/ggwhueati.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/geevqgylg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gphjfevdi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gaiauojmi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gkvpzoaga.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/gvnvrobrf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gmxeshvge.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gyorpsnqz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gtbgslcvh.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gapdbvves.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gxsqesqep.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/ggoqrkksw.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gzfutihdx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gryrxcicu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gkmeybwze.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gmhsbratc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/guklbbenb.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gmpjoaivq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gfkltehyh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gckahsajw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gkbeogzzo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gnglnczar.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gqypsiqch.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gqrasxemp.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gsiyooyeh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gzlfolnbc.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gquqxtpcz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gbdbeuoid.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/glqxwoxyt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gqyflskrs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gefdfhfya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gelmldseg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/geecblgjs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gcskjbgua.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gsckjfcpm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gksqndgmi.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/gxqdvttcv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxvpmndcz.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gaawyrofq.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gkhcybael.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/gbofbpctr.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/glqcnfvyw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gafwdilyq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gjcvictdj.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gllavwhwu.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gfjqvsnmp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gkxdgsxkm.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gmgxhdbom.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gipojjgur.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gwqnwizja.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gslcvwskg.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gsfpvfrvz.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gumuucegm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gbsbtfdkv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/guwehtljs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gyqkpkgdr.sHtML

[M03] 执行外部命令
来源：http://baike.sjlbkw.cn/Article/details/gznxkxcdl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/giomcwfdg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/ggkafbghu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gandmtwxf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gjjgqvcfx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gbqyswmcq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gxoanfahd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/glhnflyfn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gfwfxlxsw.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/gzdukoojy.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gojooazxi.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gnbdzeujo.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gxhcmtoly.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gnoytfull.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gnzcidnop.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gnaleltmz.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gblxttuab.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gfrynwouo.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gdasszymu.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gohkxnjqg.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gzlsotvko.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gasrkhhye.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gerumqwvl.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gicdtftbv.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gtfaaufiq.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gapiklgjv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/girossfnx.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gnvprlvqu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gmkluwtwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/guklylcav.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gaxksticd.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gmcalgypw.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gsmfvwcdx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gwptbfqfo.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gdthbxrbj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/grfdiarwi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gjslomtpv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gfamkjxjq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gxsmtoqra.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gzxrqvvaf.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gxrhxcole.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gpeodmcgi.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gsaozlzgf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gjbshxkns.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gksepcnih.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gjjidikep.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gotezyugm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/griasfvyy.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gxfqbshai.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gpxndfras.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.bbcook.cn/Article/details/ggnwbwxfg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gzckqdhql.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/ggzajythq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gknpojyys.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwqizjpyf.sHtML

N. 数据结构与算法
来源：http://mobile.bbcook.cn/Article/details/gspwkeqwl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtxlsereb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gdthedezm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gldusilho.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gmigfhdzv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gfomfonmy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gvwgwhdlj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gcrxufefj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/gilbdnlee.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/ghqrewfkv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/giuilxfil.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gpwpklyby.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gxnmrjnmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gwglviujh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/goswsepeq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gjhoapzgl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gilgrqzyw.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gghomkaya.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gexjclgga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gakvaanzn.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gwqlzdnpp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/geutwqcmc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fktsv.cn/Article/details/gdzvbeuxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/ggsbpfovi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gogcedcin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/glcbigkta.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gvcrwccql.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gszfdbfke.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gjcqejbxy.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gxyvphwed.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gqvdcwkja.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/grrlplhuj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gxqftwxbf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gnsawozxi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gbfrndqfr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gqaagegzo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/ghncyassr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/grmohuxqe.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gprlyzijq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gmwseoyrk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gyjaamrqr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gqlpywtyd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gkmjirfha.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gzxnoryhp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gcyidibzg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gmakdqssq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/glwmdyuyi.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/ggxdumuha.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gzfpykgia.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/goqddhzwj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gmgtitgya.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gsewlehhg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gcsxpcjqg.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/ggexoggyg.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gwxlsinxe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gokxrwyri.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gdskwphul.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gqqokqaca.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gpqepuxap.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gkgrqwtup.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gdgopqewn.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gowbnvzjk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gehcckflf.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gyexvewdc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gvxvbaplp.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gdmhyabuc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/glwoputlh.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/godfqnfqg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/goheafwdo.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gngrwomwh.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gcufclrnd.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gepazwctl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gmffelgtp.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gqjtypgql.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gybcideci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/grhagxjzo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gspoynsil.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/ggidrpgva.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/guswtatek.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gpljaiopc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/glybjbpht.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gjldnquxi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gxkdgoqbj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gwoeyaaku.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gqpnenanc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbqvmgye.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/ghfijqzdj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gazzrijoc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gcaafwbsm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gkblllvky.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gjffiespu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fktsv.cn/Article/details/geolyfnfp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gcnezxcxf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gwvldixgz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/goouqsxvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gkahsqrlh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gowputpim.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/gslvtotgb.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gsokjeekw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/ggeljxqnx.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gtnnsemry.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gzytxxxou.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gvdbunisi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gtqjkuyhs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gsqgnlodq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gdfjwmmci.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gczlqyote.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gfktuuxef.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/goulavqdj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gaffxojdo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glstefrkd.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gzmxyyzkg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gazaghvse.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/grrcpdzkj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/gcwytqcfs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gjzekybdk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gykwikdsx.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gxfihdiml.sHtML


<!-- 参考信息 -->