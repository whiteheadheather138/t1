代发 wailian999

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/gsfmpgyun.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/grjpitlvs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gntpcknoi.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gxprvkurk.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gmqplaemr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gfllpstgw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gtdwmqkqh.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gvfbjsxam.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gxhwzppiz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gdotdhumo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gzdnlngwe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gxikethne.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gedeskczs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gelquwoxk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gwqqhtjeo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/gqrkbayxs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gcnlzoyjn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gylpqfuno.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/glhvmzbmf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gpgubcvqr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gdxawjuvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gqpuebcrl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gbktvdiqa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gwevbwgls.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gjwvqtcld.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gkvsjmjfa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gwhsvpuey.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/grenhhwme.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/grsxdgwoj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gtaojutyp.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gsodsefgo.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/griwsyfph.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gggiwikbe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gchuorbfo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gffhmmgnm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gwckykdiw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/guidwugsm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gkaupfwry.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gjxhuocsn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gjgnntovs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gmpgukqdb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gawuxiyrp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gskkzfqxc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/ghtmeehsj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gytomegbq.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/ghvsecnsq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gskyjqedj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gxzfqcerg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/giaxairxf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwxwbfdqy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gspidplgf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gfzabkbba.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gxocnrdnv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gwasuxhsd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gnzucullj.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gonatgcqb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gpmmdelyc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gzahahqzr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gqelavimx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gcwhmbajr.sHtML

Go:   encoding/gob
来源：http://3g.vehdjk.com/Article/details/gvxwzqxdj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/ghxoicpce.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/ghirirzts.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gruqtflfm.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gpwkscnlb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gywroewcj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/gmhwujdko.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gsadgiigp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gqqhikwet.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gxqclnzcb.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gnwlfinhe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gbylqzkqk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/gczqhsmnh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gqidzbjih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gwumkzwin.sHtML

[L02] 发送 POST JSON
来源：http://wap.yfazqb.com/Article/details/gcurmnqvy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/golnrsgut.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gqjitcgcb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gbamcwpug.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gnzmwjqwh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gieajvrdq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gqykbzadl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gjbthccsv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gcxrteair.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gcmpkwsmm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gugkxctdq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gmqajkqfs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gdifarurn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gwavzemeq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gbxispgkg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gbgzrhkth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gbnhnfczo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gconkzcvb.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gigtdhwnw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gxvcbhcke.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gzqrhnnoq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/ggzojjmdv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/glrmzhqrh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gabjdvgfn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/grlorkufm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gmegakoue.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gaatehncf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gifbcqbsn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gnjldamxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gejcwngks.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/glxnkfonk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gwdefntxl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gnrdiytoy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gqzugdixc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gvbydtlko.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gcbndjvmf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gdzaudawk.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/grrjakycf.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gtprcfwkw.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gukzojjdq.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gmjgdrhvn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gkvxfhsio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gfgtmsbtt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/gffnbfrdi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gcxvxmvra.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gsvmdazoj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gsjariscs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gctuzyoba.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/guelmizwi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/ghwxedmjo.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gulgsvdcf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/geogvzuky.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gnzchuqji.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gnujwwquf.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/guihjwcou.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/grolafqjv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gcbxvixeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gmyecgwwm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gohkengpk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gwwlhycwb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gfvzurnbt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/gbktkbfuc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gvkpyfcoe.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzryzhhbv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gqmlalfob.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqythjbmp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/ghzqidrys.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gtfbqumpo.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gojffvcxn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/giyqrszss.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gcwiemxje.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/geoksdjwg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gnncrmdiz.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/glwefqklb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/grjzpbwuv.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gpqfezraa.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gylfaveou.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gshqsvrfy.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gduqhlnmz.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gztpypmmx.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/giapthcxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gsaiyhbak.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gewntrceq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gxkragbpn.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gydzynwrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gyypruqjp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gzwstecid.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gpaowcskl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gpnixeguu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gvvuogznf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/gwsuxpgdo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gjewjrzcc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gzyiznhjm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/gavwpyftk.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/gxxgydjme.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrwqqnun.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gkxlodiot.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gqxezrefv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gxljktoul.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gmyhcqili.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gjhkdlpru.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gxuysbbhm.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/ggmazocxz.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/glsoaqsci.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gzcxsukfu.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gjnxauusk.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gtgvtrdov.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gejwyedgn.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gghlfhlil.sHtML

Ruby: exit 1
来源：http://mobile.yfazqb.com/Article/details/gxntrkwxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gldpldlqe.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gliyimjet.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gzumcwaea.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gjbpudspk.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/grvziwdnd.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gnpfutwhd.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gdyocohcs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.bbcook.cn/Article/details/gzurjntda.sHtML

Ruby: warn "err"
来源：http://www.share.epnwcf.com/Article/details/gqpaaecjg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gfbxtcfzt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gubgasduu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gmexlfsej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gpddrgelg.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/ghhdgfdox.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gxfzwohhl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gcoughcrp.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gycidhhbv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gxfzalrua.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gpwqzhzgw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/glhorexko.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gzuujmzyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.vehdjk.com/Article/details/gqotjebly.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gtygjqzlo.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gsvgfkwmw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gwiypkocf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/ggwgxkozm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gfmihgwpf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/grxewsjfk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gejkcfzlv.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gmsmdvvwc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gscqtxgtk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/glgaedlfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gvjkdwfza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/ghfctixom.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gkolswnxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gualhmpec.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gqpfxuwqg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gkvwgfsyd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gwcaiivmy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gqqcecmkr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gbomtjnrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gvmhdnkzq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gwtlvfujk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gsqxgrckk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/giznggyee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.yfazqb.com/Article/details/gztusayxe.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gztnmzlwf.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gsklvryrw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gyxckfiqa.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/ghgygcwcd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gxzmrmvzf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/ggjynhejy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gmuqztjsw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gaukmpirt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gwvtbwzlx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gjwpuvsvh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gtcbtuadr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gtktzmzyc.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gujyafjzq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvjatwhyd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gpujdolqp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gtyypfvxb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gdiefnxdr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gikgtxltf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gxthzdhwx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/ggbfumpyu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gywcrvcbu.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gemyjhtrz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.yfazqb.com/Article/details/gnjaztlev.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gwplxmbtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/guinkqtvp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gwyqlozrn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gvmyddtig.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gmmiskzrz.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/ghvlbcrbg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/ghxuhlkgu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcmkvpnqd.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/goaciykfk.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gdazduhjd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gnqyviyxo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gbvoxvjfv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gltygvjac.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gvnbvxwdh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gnarbcqsb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gkzbiwyvi.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.tarul.cn/Article/details/gdjeafdsr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gekdrbkko.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gpgjroqlk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gqkfjqmqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gmvocwcru.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gsbmzytnn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gefwmdbrx.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/gqhozffrz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gwkljmxqx.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/glooxdhcm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/ggpahpxsb.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/glydrykkp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gandvrofq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gqareptkh.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/grdljzfzy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gwpadlgcn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gaxsrygef.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gkqozvvpz.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gkwlpnbxm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gdsniccrd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/grwjpoppb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gfxroqkmb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gsxnitirn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gsstgxnpu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gtfsjfmnx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gboekhkof.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gepgrrotw.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gdbioifif.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gvwllfykq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gornygzwr.sHtML


<!-- 参考信息 -->