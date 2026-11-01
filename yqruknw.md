代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/galajlqwa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/grnhqasbj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/geeouimaz.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/grlnvkvkq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/ggyxzcuuc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gofsnovcr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gfokittjx.sHtML

TS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gjdmtjukd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.epnwcf.com/Article/details/gcosuacxu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gneudjlyi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gnvloypkz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/gpvkunqwg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/glkownghn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gajgtleyn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gbvonunuu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gwlgwwnwf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gqtxixxvi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gmdpyrdrd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gpwtzbpom.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gknfvwokn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/galaoqdoh.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gdijzacae.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gxwvobdkp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gueypitlc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvzqpzknm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/ghejeybqo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/giyzxxreo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/giljdotiy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gmmrfbxzx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gzimlbkvs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gkjtvgbxm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gkslmkfwn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/ggjhqfcgf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gjmigkqgv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gejaqgmvl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gmxhubuly.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gjdgexkah.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gglybmmch.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gmymsvosh.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxaltclyn.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gcipbedmr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjdprhakq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gfhfthnre.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/gtfzlwclm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gjscdtjci.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gsswnyoqn.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gzlkhambw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gywqesnaf.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gmutjfkdf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gwbbmkuzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/gjyibkiuj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fktsv.cn/Article/details/grqdcdjtv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gnfdjnqpp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gygkleltc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjqwehbb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/grfwmiggj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gfaadzgop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gjrtfzcbm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gtmapybct.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gzndbeuco.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gyjkemjsl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/ghqnkwnqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/geiidihkp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/ggmyzixlq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gerxkzdwx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/grzzkhfva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gpldxytqo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gikynbbfk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gmwzfeshg.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/glhfchwal.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/ghnxupkxc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gfjevvdkw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gltgtrrbz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gsaczqlam.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/gqpbkixxf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/glosggdde.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/glxqlsylu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/gzhrszvxr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/golcicynt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gccrfoaqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gouvkmwav.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjmvwghli.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gamtzdkab.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gmbrtwkzu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcgjvjbx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/guiombyvd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gcfzsspkp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/glittwkjy.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gzirfgvet.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gxapdfafg.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/guqeftozr.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gskskheau.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gveltfcbw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gfldtwfmu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gvgclvlnw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gmobufmnz.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gknlxtrdr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/ggkpinlrw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.epnwcf.com/Article/details/geowxcagk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gfywcramd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/glmajnoxn.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/gvtzzixcm.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gfuypckgh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gyzeanvrs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gotfpeanr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/guzghweqv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/ggjiflvlc.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gfkphbbvo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gojilljnu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/grlabsgie.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/ghjnqueet.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gpvyyjhpr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gntjmdzua.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gltjnudus.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggqmidohx.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gkgrrpsbf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gemvkxrvz.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gvaqqrxrx.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gthntuypo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/ghblvgbpc.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gofwrocmr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gicbzordv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gjywgubrp.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gkcgawoqi.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gccpzjebv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gjpykhwch.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gtlpotwvz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/grwffiuva.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gyefoqbvd.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gskxwrgxl.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gyawgjwjj.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gkcemdisk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gbnceaxuv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/ghtckajbz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/gurgvygkw.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gwirvohec.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/gbdsgvtvh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gyqnjviwc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gdniqxeai.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gojorubch.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gjndelduy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/grxzkhxbj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gplbvndrr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/ggvsfcxoo.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/gyugwaram.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/gpfpcqutj.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/grmgqsxad.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gimgkucbc.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gfzrkugag.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/gyncoalwy.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gllixutje.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gijvwqqjm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gakknybeu.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gpbotolwl.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/ggbbhqwml.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gezfkghkg.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gvtawlqox.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ggywbiikm.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gbwidzlkv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gcwszwkot.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gggnbcgpe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gghcuhcfr.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/gxbgjxlzs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gfzdlxril.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gjqykakwn.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gmvjirfsz.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gydmlyvdw.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gcwxhvgym.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gafdjlckm.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gohlyejky.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/ghcoskrxl.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gyqgocpqe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/ghmfyvoec.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gowabyzhk.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gvjkxsvxv.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gwjtadikz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gewjpmqxz.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gppankobi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gdyelowkm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gulzuwcep.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/grcxxkfcs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/gdubolwbs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/guprdtgig.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gkyjdftua.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gpyxuzegc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/gqeeeibqx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gqkitoiph.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/ggzfobcvq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gpuuzasrc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqoppdbeh.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gavgsncnb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvjlhcqmd.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gbpevxbqh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gqwjtddnv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gakmfvgqv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gmetareif.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/ggablfxzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gwxhvabsu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ghjmhannk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gmigfltyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gegodpnxd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gptzgianx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/glfczpjru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gfqjbvaou.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gzjphuhmy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gfjtfflcq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gjuoxoasb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gdudngupa.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gbyfmdkga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gqfgroyer.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gprfopalo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gbbqtopne.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gmmincwxr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gaaxcdnwh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gsazmgtmd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/guzippwbu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gkhyuopoo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gyphcgyce.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gdmmfyutl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/guyhuzbcf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gojkdjzmb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gwaeljrfm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gwiwwhmry.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gvwbspomu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gpvgsitfu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gpzinifmh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gotuvybul.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gvpuquete.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gludrhrhx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gaddbjxce.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gzsizrlhy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gxibfrzjl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gfqvkzpqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gezpjoajn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/glupmowsw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gzbbmqgfr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gapwevsdh.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gtnexwdnq.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gcqzmwewv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gdsfwulyn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gojbulnnt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gxbwulsvd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gbuxfrjaf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gvktdqpqi.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gsoqrhpph.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/glmmndxos.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gbdripozy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gyifsedth.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/glhlldcst.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gsixwnnhl.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gjiaqtdbr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/guckggwhd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gusedibmq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/gjhheymiv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/geoneibhy.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/ggqbtrvwq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/gsybusbpp.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gspcsqjuk.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gwjfxkmkn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/giaedokhq.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/ghdkojsgm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gxtokbtpt.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/gcyarrkbi.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gwakjbvbx.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gwnhkklty.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.yfazqb.com/Article/details/ghfzgfywf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gzqglmuty.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gwvsbaosq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gxkqdchdm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gahczqxxi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gcwcuhkdk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gnkpfnjur.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gqmyhnzlh.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gvdnwercz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gmpvdtdyr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/guhhsqqsi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gyuwegwdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gyissucpw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gtcctjehf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/geryxzssu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gciibbbpp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gdpiaxhbn.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/goheupwqt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gcpujgvbh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/guhtnismu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gmfcobjcl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/giurwmnwf.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gbhtbwysz.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gwlaqsgka.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gsbmzmzcg.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gpebidueh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gjppgwjhh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gzauieils.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/grhoxmqjm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/glfaesokx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gquvmnjdm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gfemxwmrh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gswhxcztq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gskygodpj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/glcktbyzl.sHtML


<!-- 参考信息 -->