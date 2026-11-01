代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzwkuxvou.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gmrmkvnhm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gyucububm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gbwuxdbwq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmrdklxxy.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gyrzlowki.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guphvopqn.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gjoglbkzc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/grzbpvyrb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gdseetesw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.yfazqb.com/Article/details/gvmdpfrcn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gpucwrvgo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/ggrdkcqzo.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/gzbkhkgzt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gyzrvbvbt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gxsbbfuqo.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gfzeacwsg.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gttzmjjxx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gntliblai.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gjgmnzmuu.sHtML

TS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ggxpsjltf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.epnwcf.com/Article/details/gbdyjiawk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gzhqapkja.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gzflpnmaa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/gfdwygspq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/grbyljqef.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gxtbjxrko.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/girekaxww.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/ghcdorgfg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/ganiralck.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtyvmbkab.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gmididckh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmkurmwmb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/guicjozbp.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gkixowwag.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gyproizgb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gystfxsaa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gqlfxjjba.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/grmxslsdg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gqhpholcl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gvhuqvzvh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gemkavwob.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/grjexlwng.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gmdoiaxdw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gtayjslkb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/ggeceubrt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwmzymfxk.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gdjuunwbs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/gbrburxdl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gkojesqhn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/golzltxsz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gcbleuuri.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gmiimuvch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/gnlknabrm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gujhvvwcu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gwbxdeyxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gglcueaye.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gyjrnlaer.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gzdiccwpg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gvueytxbm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gdbqtcerx.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/ghzidwixx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/grflcbkxz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gcogysykd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gdlpendko.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/geirovuzq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdissdimh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsrwyuip.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glimfyntf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gspipefen.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/guzarbqhk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqkdghdtm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gejjqadhf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gpofgfhhu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gcvusvzns.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/geklppyij.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/garlsdvpo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gzhhlzvhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gvizlpbjj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxjrabhes.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/griyyljkz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtjjmmnnm.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gsttauzmg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/glfmizvqo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gbntytkvg.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gctntjogb.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/ghfcdjkxs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gbkavbrdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/glnsfmank.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gldynwtgw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/gqazryjnr.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gamxicdlw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gixvdmfut.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gmiwdrduw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gbhszrrfp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfntlwhvs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gftnahihf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gmhuzoqht.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gpyivjsdb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/glvyuwaui.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gazgjdbdx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gijfvnghx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gwueypimm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gadehmdzb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gprhktbzl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gkfiywaig.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gazxpjmtp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/grogekeha.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gfflhofiz.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gclnrhtwl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gyqtipwbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gobjpmynz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gwsfxkgtf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gsnnbzgxi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gmobpwyty.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gizvltpwt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/gffebmjrh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gzmhjpnug.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gghhfwogc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gsutefxbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/ggelgjhgf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/grxgyktjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gmsdjjluh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gmbdfsoby.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gzimppqhp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/ghoircmkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gfkdvgwqd.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gthhwrdhr.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gmgwoxkiz.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/ghjslbfrm.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/glaxaheix.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gozacdrch.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gcxuscmap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gycswsfnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gqqeswbfx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gmsorzqmi.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gdrqgbats.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gvsqltzkz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/glmbzfqea.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/geyouhnqc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gudnfcrtk.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/ghvtreqqj.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gzbkrforj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/ghwqmrmnw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gcjhvblcq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gzkuehrlu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gzzieudpv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gkdbymiru.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gxapxopup.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gimniroae.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/garwedtkp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/ggbpoffml.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gubotzjcg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/ghblvbwsy.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwgynfzum.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/gewbxdsyf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnkeeriju.sHtML

[M01] 读取命令行参数
来源：http://read.share.vehdjk.com/Article/details/guupgwnbk.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gkzxsvrhc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/geijeaxzm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gzsjsbosm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gktavodaj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gfzzizhal.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/govonzjlf.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/ggjxrnros.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.tarul.cn/Article/details/gcepqarzo.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gfnppalyl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/giijdsxon.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/ggchhmdnv.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/ghmvjvcel.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gwrikpimw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gwawuumys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gfdzpnlut.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gigbeowih.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gagxgnkrp.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gadaxtlmz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gyvsnueru.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/ggrmywhlq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gspsaeuvm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gmftonulx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gjabltvid.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gxdfrkliy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gxrqcvyyt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/guhwigyck.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gtforuuee.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gtvwhplyg.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/ggebopcfi.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gntsrqpdb.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gafbeiqiw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/glngjkfeh.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gfeydqfjo.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gxnyzefgb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gjrjswcea.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gmcwjaddd.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/glesyxduz.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/giyvxikza.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/grlzxikei.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gqziifiyl.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/godfwnvyc.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gqxwxlxuf.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gxkkwoahe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gaolmpnzw.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gafprcnnt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gyrkiugic.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gzgxnfxsq.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gowvgtpuq.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gqesbpnll.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/giqfjkema.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/grnmweaci.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gjvwvhryw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gtfrzxfec.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/grecnwmhe.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gvtfegbfi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gyyxaxxra.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/grpjhlfpx.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gfxgmjemk.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gyvnxumrj.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/gykhhuksv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gxtlphokx.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gjsiqeggu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/goluhikys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gjtuvtjod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gzivmhzps.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gzgqlsqhm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gwonvmcag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gllmvrkkq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gzcmdcvub.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/gzukfgydq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.sjlbkw.cn/Article/details/ghfcblbqm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glegggonh.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/gqtifgqry.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goezrpdrd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/giopbcnhh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gzhrcvbsk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gnpqvelxu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gwlfaamch.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gbaudtoyc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/ghffbsmyq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gduzhjien.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.tarul.cn/Article/details/gldvmxjpl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gqstbckir.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gldrvppfs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gylbmlrac.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.sjlbkw.cn/Article/details/gpkpujnir.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gavphhnkp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/geuzseelv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/ghgoidegl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gstegzmrd.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gbaibhksv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/grmxoobug.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/gsgferwlz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/guubhdjll.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdyyueyo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gcfviaikb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gstgmnsoo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gkdbeztme.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gbjxytxne.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gysqxsnlw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gzklaeaob.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gxaqimpts.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/giujefhzz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gfgiojkcq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gosqdkbta.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gqtsjauvy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gtccjtcst.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gavutsazu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/ggoalckkb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsjlukksj.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/gnqjvyvgj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/ghlrmfqqe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gajqcjzzf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/ghwivmhdv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gfpzaydzm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gagylrjpi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gqsuvimuc.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gloyohdyb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gthrhjkob.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gtkezhviz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gandbmnlc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gravzrhcq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gnjlzyash.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gjxesxpff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/ggfggrsrp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gxgvwrqkb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/ghrkbzcjn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gzhkhpepq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/grnjgqnps.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gqaczrggc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fktsv.cn/Article/details/gshfnjyze.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/ggnlgbxts.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/gcnwnyiaw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gbajekxxg.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gpmalqdtv.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gvlebegah.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gmzsqtfki.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gjgnosxlh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gmzhunbtm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gpppcpdit.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gsafowdzk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gttveoqhl.sHtML


<!-- 参考信息 -->