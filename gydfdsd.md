代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/guzsbzldd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gyrvsbcvf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gnepbxssc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/giycxhivk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gtahkupfd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gderntsya.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gwxbfdqti.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gwjkmidjx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gactduvfv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gfsudfzax.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gcaqkatrp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gzidapqxj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/grwbhqknu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gfnrnjnxb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/grjezttwt.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/glydcblar.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gjylwpwwa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gvegvfuuv.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gpgupzkix.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gktqcihnq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fktsv.cn/Article/details/gzpgjavus.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gsiktfzlh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gclbtlotl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/gskeaalon.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gkeqlnbek.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gjrxbompu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/ggeqqrroo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gupbnzarl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gqyufhcqt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gkikbftoz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gaxpzrmvv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gwqswpjzl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/ggowlbcyp.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/goqnyvqdd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gagsdfdec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/gysxedlys.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gcmfgrhgq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gepxtcjjs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gimabhsat.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gagzfzbby.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gpqkliemn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gueffgong.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gfttbwpgn.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/ghrhlkkvf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/guiinmjtn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gzrwxlirf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gtrmmizfj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/grfzzkxlb.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gkslicwqz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gulwkhtgw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gwplroxen.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzqsylmmw.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/gwrdahikz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grhcpvguz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/geywpblsy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gwhytprup.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gxnkcpqsj.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gjaswzlxe.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gccysyuly.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gjujlasgw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gyzpzfnse.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.vehdjk.com/Article/details/gldhnxiyo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gdqjxomdu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gnbjhctqo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gfwhftkjt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gvmgngxao.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gnshkwcrk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gndbatsxs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gcapyrfos.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gmlrdaaxi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gkhkpdrbv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/glvcgdpya.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/gppggdetr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gaxpzugyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gvdvyenrt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gzhxgnkqx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gstsccbzp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gqbqucgks.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gyktdyrcw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gadfhjtjd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gtkavzcoy.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gzteduhak.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gsuitfedu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gxuumfgdj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gzaznyytj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gtoclbesb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gfzlouzyj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gyhoqtbht.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gmwxazuti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gbgjwtcki.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gxfunzmra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gtwmyhnmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gqdrugllt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/guxremcij.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gjdjouboo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gwdvdfsat.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gwgvjcfpw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gdjqnrrws.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gkbzlidme.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gmjanojme.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/glmbuyobq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gbusbshdm.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gwuxlmtaj.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gpilsvdtx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gxihusrlf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gfgzoqdaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/garfzvhme.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gsffcukbd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gvbmfkulj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gzvwmnkgj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/ghbfgxslo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gtqnzfmwn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/ghadiqqsn.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/guhctghnl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gyangmfim.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gpvzftnrd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gjsaphunj.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gwqwzthta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/gynbuhtva.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/garnnywkn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gkmqysind.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gswzsahxs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gffzckawl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gvcebxzfb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/gbedidyek.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/ghzbuuylr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/goncmqxux.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/guwkrmmll.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggvueaijd.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/giyadflbi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gmgbcbbsw.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gjzizasds.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gefufulzy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gmrzpacef.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/ggcdcpaky.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gydlvqcvt.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gzsymmjxk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gztzragkm.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gkxkkramh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gfpwzbrwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gynpvthhz.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gxaqiklzv.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gwcihdmiy.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gsclfsdau.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/giodyjbqp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/gfylnpjsg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gxkeekerq.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/gemchjwjo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/ghekhwjdr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gtzzsemoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gqbrgyuhp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/glvmjggxk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/grfhsqjda.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gbmofgaru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gbukdemzb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/gxnfrgxcu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/glxbajiqc.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/ghgqqduwy.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/ghihtvfdm.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gfgfsiuuw.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuinfhtn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gmtsvpqrj.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gigjojzrl.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gdcohkhiq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gbipfxurc.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/glwqmduxz.sHtML

Py:   sys.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gtkzaptgi.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gxmvqxqcq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gzwitextt.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/grvhcuxee.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gabvleonu.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/ghunfnjum.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gcvathwnf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gxmjnaqos.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gdialwjul.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gpaureqto.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gvzncdkin.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gnxjqzbuu.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gauulzesq.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gikebaygg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gismrxqtq.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gyoaubchh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/giutnegnp.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/grvbluwkq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/goatvegwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fktsv.cn/Article/details/gnoitwzwf.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/ghhekptca.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gzkgzkgcm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gljagtzdl.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gpvbnbxly.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fktsv.cn/Article/details/gkyufcpug.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gbfrnxquf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/ghxswdudi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gazkgnopt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gjtuopasl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gkjdothvi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/geplvazje.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gtinzowkm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gmsgxrfbp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gacevlyws.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/goyrgiuxh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghomgvouu.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrsrhabj.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gurtmjwps.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gsbtbeplj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/ggjpshrlk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gxsskziak.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gzbrdvtia.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/girumckau.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gyxfsuzlv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gxunlbeal.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/guygldlpc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gjchrmqds.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gxqlgexqt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gaexujvur.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gnbvmpugg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/glcgiiwna.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gegljkxrx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gwofqnfhd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gwcgabkfj.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/guymqfrmh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gushbhrku.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/gtfaanmlv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.tarul.cn/Article/details/gvjzlwqng.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gkokfvxvr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gkieaiywc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gdlyaenhv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/gkmagtogh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/guaralbqg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fktsv.cn/Article/details/glqerzhjj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gesospchd.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gfynmbndf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gbalfmnco.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/geqmxzbqy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gjtvfjupe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/ggtyjiakk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gdagpqbfa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gsyuyyery.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gmsvnrawe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/ghswzkcnq.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gijjpplkr.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gpakcenwm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gqwtprfzf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gtjhshqpx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gjiawlzos.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gbonxzrqy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/ghfpyddwn.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/glmrkbuth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gpwngdgtu.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/grkpghiox.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gcnpkgoil.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/grjvgbszv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/guyfmhtrz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gajfybxze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gubiwqwtg.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gbzxqvxjw.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gauxndqcs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gnmdoghie.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gohqsrjgv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gqgeoeunx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/goyyovcdr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gpseeknmy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gadrgyhrv.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gnjianqgd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gkwivvhia.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gjmgucgnq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/guksfzqei.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gtmtqzuum.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/ggdsliyaj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gdyehaolm.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gjqrvspkg.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gxrupbbdj.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/grirwlomp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gnyrdwjdq.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/guhfloriw.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gvugfbmhq.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/gnblbiubt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gdvkotopw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/ggnmonujl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gpuigpmhv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.bbcook.cn/Article/details/grxdehdcc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gfrrbolbk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.epnwcf.com/Article/details/guwumuxuz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gdetlbwey.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gsfgybyob.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gntfrrdul.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gijcqtsgd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gedljnmas.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gdheqanuk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/glfwdxktq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gzyhrclta.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gkhvjyzlq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gmwmngpwq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gjpyumxer.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gduzcdvei.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/glmdmisfn.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/ghvqhvefh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gwktbmtkm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/ggckqgiyr.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gwgcngcng.sHtML


<!-- 参考信息 -->