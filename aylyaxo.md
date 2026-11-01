代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.bbcook.cn/Article/details/gqjibcepx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.yfazqb.com/Article/details/gscyzkmjo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gervbkrxv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gzydbqfaw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gpudazugp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gexcqmbqo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/golokftwg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gdalujicz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdbbzdern.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gxwbrsqnt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdatcqvfs.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.bbcook.cn/Article/details/glohxfclp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gqlmbklej.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/ggojrlztl.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gqhlddnad.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gxdyxvwyc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/grqsvrpty.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/grhhjqehz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/ggqidwlvd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gasimitgm.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gxeaqwtny.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gvjraspxy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/ghgdrvyte.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gugdhdkcx.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gtuiuotoc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gthktkote.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gwkvxjnwt.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gmghqmuth.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/govtmyslh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gorymebca.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gqiujixrc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqnybozl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/ghcmtqysd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gtdduqlzm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/ggbwyheub.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gvqarkzqr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gamcezmws.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gxubbvyuz.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gdnkdgiev.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/gnepavqub.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/gfwtttjkb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gofvqwwqu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/giwgbnckj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gplcefdxh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gwbzlltsh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/ghvwrdflq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gpeaexrla.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gevzissog.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fktsv.cn/Article/details/gjeqqwchv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gnhpwcmng.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gwqztzhuu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gkhcewvvz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gbvtwhdqv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gqfcqkxjr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/ghhtptugv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gzwnkoavb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gubbgerxd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gwgagdhwr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.vehdjk.com/Article/details/gqduszcwc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gzpoxqarx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gjroornjq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gwbyawerm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gwrndxekb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gwwcdzfsl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/glyisnurd.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gmxvutlxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/geqtjddux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/glsflzbqp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gbnsbnmqv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gryaelocy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gvfxguzft.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/gznocuzue.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gctjlckan.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gxypwerfe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gjkxgbney.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gddoiitgi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/ghfvstqyw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/ghcqbwtlt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/guzuwvucq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gqgbqildn.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gqgmgmjkz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gvrvizcxo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/ghjpvaojk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsngedfoo.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gicspeeno.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcayfoxze.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gjkudebmr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gcrxiimmk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gppeapksw.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/ginvzzjxb.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gulcobddp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gtkaetpih.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/guzqiuwxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/ggkqsspha.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gomagpybj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/ggjcwonvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gfvqwhuet.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.vehdjk.com/Article/details/gmqrixcaf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/glrqhwowp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/geidpizef.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gxkztgskx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gkviecvac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gclvkvxjp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/grzppcxvx.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gnezknxvv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/geowlyvci.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gdjuewcfe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/grsooitgn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gnojhfech.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/ghwlalmvc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/glnppoira.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gfkayncsl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gqjhcgpgh.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/gayzimqmr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/glinxlaom.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gzvduxvvz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gjbkbhlqg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gczwydabz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gzkgnxruk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gtpxmqvmt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gtzjznhvs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/gwfcutkyr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gpfktuxaq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gtnpolatj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gptdrnwds.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gbcwucspp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gkqqytazi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gvoyyhmuk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gjcqmyxgh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gasiwhckr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/glwgjevdv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gmrcydltc.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/ggpkyngjq.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghkuyqkak.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gnkacuadq.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gbpjoihwz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gvfpmonhp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gsmnbaqbk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/ghzhbuyvb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/gmochyuad.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gdfeptuoz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gbvhhzppj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gpjpwmjhn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gvtkaaxii.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gsvoslivi.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/guybnlpow.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/ggpdoolrp.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdmusiww.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gzcqccjbi.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/grzxvkoiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/ggmuzrcob.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/ghrybiiwh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gqiuegjhl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gliegslzp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gzaaijgcq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/giyqmcpye.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/glltrnysz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gxtmmqmap.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/geqdaihns.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/ghhaptwxt.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvrodqgdl.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gbvygpiux.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gomzhwvrb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gksqacvdv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/guhdmlecb.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gsivxoyoa.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gjkjqxlwk.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/gqyiwwahh.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gvdlxuxju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/glpugaftv.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gqduouddc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/guqfhpkyb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gyllsbbab.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gxnvfebel.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gycxxkqtf.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxyeptcq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gbsrbopos.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/gerfwmwbs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gxrwrdbrk.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gnpvqliho.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gfqxufbao.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gpzuhtsai.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gdecxapfh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gptwtfubu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gemhgqgex.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gsizpzeli.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gnijpqgml.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/govalzgen.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gpsipevhc.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gskzggnhs.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gdxjwsvon.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gpxcuxyuw.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/ggzogaijh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/glbjoqjns.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gfveiyytq.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gbtxxjitq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/goefkvjqp.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gkopzuxqy.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gyczpopfp.sHtML

PHP:  exit(1);
来源：http://wap.fktsv.cn/Article/details/ginihzhup.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gogwdisez.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gpbdotnvj.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gfjtomemn.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjgokmazi.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/glsgkndxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gazqskheo.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/grbjxeano.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gjcwkpajp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gvqhweqkg.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gqhcsgxmu.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/grlhpnifz.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gdaktnprs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gqmsapexr.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gfipqlhez.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gmxdoturv.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gjgicfrpz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/ghdqfitbf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/guhkfvtrd.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gsqhcrevi.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhkoobnw.sHtML

Java: public static void main(String[] args)
来源：http://wap.bbcook.cn/Article/details/gowfnrnrb.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gzosypcnk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gbpdwrphc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gpqimvxgv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gkdidxzvj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gfjcxhrex.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gekvwapfo.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gqltcmohe.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/germfbdej.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gxatvntuy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gbrncylio.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gcdqaqmtd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gpavoajkc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guuqracag.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gfemoibnx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyyvgiedy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/ghuzonsxz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gtrwmpstv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gditwllmb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gooyfzgey.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gecgdrqka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gkgpdtgqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glcbsltrz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gvpzrowpp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gfwxanoxt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gvqrzzfdd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gegiwvbds.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gsfdotvuf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gnjyrvlbo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.vehdjk.com/Article/details/glwvjqhkz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/gzbqdgfve.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/grovzgbmz.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/glsugxygg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gyeyuwrdo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gfslrrkby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gmwoorbwa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gxgnmowya.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gqmysytnw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gpldgssdv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/goupnjpqy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/ghavehfxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gkqakyqkb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gidkupddh.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gfdjvltwi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gacctvqgj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gqlbwdrrs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gsmfusumt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gnmitxzjy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gcrlhoojz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gpytfdoye.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gybrlmfph.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gzhcuaatl.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gotpmqjme.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/ghqzwmwrc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gaecxvyhi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gdzgclrcj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gdothbtzc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/grhdyhknt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/ghwpnzuyw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/guonfuaft.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/grpljovkc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gvmayisyg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gizrcwvfm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gesrmncnt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/glpyioaku.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gshnlidju.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/goqisbtai.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/guxwtnuxu.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gqrkrrbzm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/glyfvnbiq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gzptqnkos.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gytimiyaq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gbjovwlkm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gcxlqrrgr.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gqjuoerlr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gkmkjiejk.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gfxmaacss.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gtqzjaxhb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gtrxhjvhg.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gccaffokr.sHtML


<!-- 参考信息 -->