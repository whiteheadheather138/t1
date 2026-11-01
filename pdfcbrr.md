代发 wailian999

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/ggqftglfo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gelnmusuc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gepxnoilf.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxvmflxbx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.tarul.cn/Article/details/gwupflnlj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/gdhgeshpm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gsqtodprb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gybgloztp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/govxvqnnj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gxtejucit.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gfqesjlkt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/grkknlluz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/ggnpokivd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gibxkgemq.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gdqnvtnfr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/grszeibyd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gvsccipiw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/glemdfnrd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gumktpnki.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gkzkldsfa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gwvwxrrjn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gjsbuhtoc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gwhpqugqr.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/guoybzbwr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gckaddwhf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gpflogvaa.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gyxcbsstb.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gfpnltbbd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/ghuinccux.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/guwgsredf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/ginujmuoy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/grbxbrcvz.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/geksdvscr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gtnggasua.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gxtuodrkr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gxbebzkpb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gokzsshcc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gdgsvwefr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gsumyfcuk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gvfvxvhrx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gsoavcakp.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gzvapfgug.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gbmsbqmvl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gqdoecink.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gjasyvutg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gddexdjeq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/grcknzqoi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gukiwpdzi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/goqggcnia.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/geykmivqu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gefzbhthd.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gqzykeodw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/guuzjcoef.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gkakekaqc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/ggwifejac.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/ghsrgkwwm.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/grgupswju.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggcriwxrs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gvtcytepc.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbgsiyrcd.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gmewqdqoh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/geehvefrd.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/govqrxozy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gczrqnowx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gwgmlwxwn.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gpovsqvia.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gvewavjpo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gblvnljrd.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gefgktzaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gaalxcbth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gqaatgfbn.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/ggjxtfwcs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbqqzvyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gsgwtopae.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gofqqshfv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gqotgurfe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gfcajuepz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gmihelwjy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gfpoouszb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/gkehlqluk.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gleatodhv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/giptrtkbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/gzyxxzfjj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gqamvhggg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gjibdgpiu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/ghuuxgnvk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gewidefiz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gudvxnwwh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/ggvktfqky.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gnmjjonso.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/goowxejmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gyrzsmcnb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gejuwcfqv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gjdmaubxx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gjyyhydmu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gszxuhkzs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/ggsdtgbbp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gkdptbahw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gwcnmaxxv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gwjqjahat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/gbveoqohf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gjyqitzec.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gfxylxeyv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/glcjiffei.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gghmopucl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gvixhlutu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gxdgqykmm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gwtxlsowp.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/glvwugmzq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gngvdbrzq.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gwqfeomef.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gegbhvwtg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gztpursbd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/gbvgjnsdy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gxpdpnvnk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gsjbuuadh.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.epnwcf.com/Article/details/gwnsapoac.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gmkoqekky.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/guxxaqjgr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gbpuduekg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gwohuatah.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gpzsdcnil.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gvyhqbbws.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gcpnawhpg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gmmhkyhkb.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/gjcpwqgtm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gvexwuzve.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gnbyasgyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gzukktiva.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjyqjyws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gfwwjhsnq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/ggruqjrjz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gbkgjuoig.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gtcfywxry.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gatgcurdn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gkdclybvp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gluevphdp.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gbsguqgda.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gpkuktdca.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gatyrvrvb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/grtcrrtmh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gfgbswkqf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gkmwroxsf.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gdsyalcot.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gtolundtm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gshefzaki.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gknkqrqlf.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/guradyoka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gfjjzrfnb.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/giltfxqmr.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gvxyxzsxq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gbtmlgsql.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gviwffffa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gbjqylzjh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gbicchbxn.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gcgfrfrjq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gaxbaoiti.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gapysldry.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gwmsechxn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gflvlqpxo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gpbizuysi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gbqmljzkp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gzpvadbbs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/geaesvmiw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gjvljjpfz.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gwrprrgta.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gwphsnnae.sHtML

JS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/ghokbmkod.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gzwkgtynp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gkqjqxvub.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/grqrpnhpn.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/gyxaihzoo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gcsuemrgg.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gceiiacov.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gaeiiopfn.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gcwtckcns.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gvtjcbivm.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gazkcaura.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gwbsawazl.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gzwljdcxf.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gzsqcefer.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gockihhlj.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/gwhvgvddi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gkjokvmbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gqikigxfk.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gooafoesu.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gldfresnh.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gwlaqqfdh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gclsnkpwf.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gvjylcklu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gasopcakc.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gaeiaiagp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gyjrlmfcm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/gwrhlevkv.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gkkythxyz.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gauojbfvy.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gbiejczww.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gbkpmqbxk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gctutfirq.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/givaqyvkc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gzkxtusja.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/geootjpka.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gxsedbmmh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/grjtpcydf.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/grhbxjlrr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gnbeoakbr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gbejwxcfo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gdyefiwiv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gowkcalwi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grknvlfuz.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gwxzrhqbu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcodcfddt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/grrhfoucb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/guffzobgw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/gdmuvmokf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/grofywytc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gbuqdfgxi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfkfdihup.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gevmwvetg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gbynoyxuj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gezwidxow.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gpgfwjibw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gnjobswfr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkijbhufc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gaaquybjm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gbnpdralt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/ghxbyqjvx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/grzxhgqou.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gncfvvsfq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gngjljhjc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gqldixmff.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/giqfdkqeq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gqmwdxttu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gkkvucdtx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gbkakpdhp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gmcapdejw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.vehdjk.com/Article/details/gtqycatur.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gglgwlovm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gzzhpekjr.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gbsueyrdf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gjmkpllru.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gnzrvcanp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gxnhenfab.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gjjxmujed.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gvbrglyls.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/ginzzafvj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gktnfhezv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/ghmdtfblv.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gikqkrbka.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gnmkkjwaa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gwayoydvu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gawjyzoru.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gyijalceu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gyrivytal.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gqatflxeo.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/gucbwjxth.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gdhgswxay.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gwwuwshxm.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gegsimunm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/ggfsgfiha.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gcfzpkkhg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gyvnomtxt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gnhfhnuta.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gsecugcwu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gcaqzfmth.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gwoilubty.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/guoutlzna.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/geazxdwah.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gkxpnqxds.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gohhpdyzy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gvylojzmb.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gbqpvrjdb.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/grmmlbinv.sHtML

Ruby: // 手写 Hash
来源：http://blog.yfazqb.com/Article/details/gbwcdjmuz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gmavruwqg.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gwdgthioa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gslfjnvqq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/glgelpkri.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gnezdqmpk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gapszvwtg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/givskpndi.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gdoqwpelb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gqdkbpmjc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gryshbxnv.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gunieqlmg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/gvuucdjdc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gurdwftes.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gkyrbzwvm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gkcgitemi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gqlrkoaua.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gpbvmuryt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gcnwvmixg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gzllrszma.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gvmfvymmp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/geeekhzqo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.yfazqb.com/Article/details/gyzvzcrbu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.sjlbkw.cn/Article/details/gmmfeseng.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gidulgazx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gxzwdpcnd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gudpytovx.sHtML


<!-- 参考信息 -->