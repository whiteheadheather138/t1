代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gzxrtfoyg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gqaxotlkw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gdfsdpqgq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gubttvgen.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gjwfljyvb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/grhuycxis.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gvpcqeips.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/goyrbwsmh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gwztvqjtv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gqfyimgbm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/gcriqiakh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/gavxwajyz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/grgcuwvqm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/grhtfkfhh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gajxqlfrb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gaudbtevr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwyuznply.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gxlxcqzem.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gezijvvhg.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/gseduugrb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gfssrxfkb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gfjmyreru.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gmqedgprx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gkejyvdgz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gaovcoxjf.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gztwjemcv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gnprgnduf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzesfdsxr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gzsisznxr.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gdirsuuow.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gmgavssqj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/ghmlwekiz.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gahxnddss.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/gptwmwaqz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gyterhatu.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gpzdyrgfs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/ggttrshpl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/govapxbuf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/glibhvgmc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/guvdgazhl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbjtymysa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gzctuubfu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gamlwmaek.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gbmxxnkui.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmmxocvan.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gzqoczjnl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gaslnlgps.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/grhmrzrdq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/grvocgeci.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/glrnczkwv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gshhnfkiw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/goqdjchod.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gjjwtczpu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gkjvocfwc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gyqghapiv.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gvsiboyai.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gpunfpdjl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/gkjpazrho.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gyqfinhof.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/glhfktdjy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gzpjoncmi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/ggagvsfwl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gyeaplxlk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gnfoetexn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gqapxdpog.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gtsnpdiqn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/ghsnkrizp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gezyphmhl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gmxuyiiaa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gxgiajdlz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gxhhnzgkd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gonmvxybr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gzetbnbgf.sHtML

[K07] 进制转换
来源：http://m.share.vehdjk.com/Article/details/gxgkpzdxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gtjvbcwza.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gdhbfgecs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gcafinqay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gyuphpvyg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gywmvdaud.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/govxrgdzn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gvxuigjcv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gshyhpvhb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gsasnjrct.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/glgipdrlj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/glnsztzry.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gbgkphwzy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gmbkkczsn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gwnfczcrp.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gwokpidum.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/gphoowzjj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gfydkuqks.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdzdqifri.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gdpvxkjlw.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcnvgktzs.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gkvobuanf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/ggjmsdqxx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gyvcqubog.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gkewammnc.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gqjcicikx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.bbcook.cn/Article/details/gnudxjeet.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gsqzihaez.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/geczroxvy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.tarul.cn/Article/details/gjxyypvdy.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gsrkbamor.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gnyulrths.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gswepuqdi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gjwaerlsi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/geqefhghz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/ggpyemiyr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gtnfrhqnx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gqlysvils.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/gzcmhaphd.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/ghfvgyyae.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/gkwjkvqco.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.tarul.cn/Article/details/garnynvqa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/ggjjrwzyd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gioblgmlq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/glnwdwsug.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gqjtegqkf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gaptmqame.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gwensnela.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gkieplpkp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gulsyskmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/ggwrwrzij.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/getbhomdk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gckzmpoml.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gukqpibjg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gafmcnztg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gcivjvyfw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gwgpmbgmc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gvsufgqjm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.yfazqb.com/Article/details/gwnbnblpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gvxirlrtg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gpcuppdcx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gfbaavotl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gbqmsszac.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/ghwfmehrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gwrjtjryb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gatrzmxjk.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gjnlgxzkj.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gqwbzrpqc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gxoyxcotw.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gxpqpnwpa.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/grodiusir.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gwjyocoob.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/goupmybsy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fktsv.cn/Article/details/gtjkksxfa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gqmxghrdh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gqvedmexh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/gytiypomw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/ggazueera.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gdaetzmmu.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/ggvgkiyzu.sHtML

Java: resp.statusCode()
来源：http://wap.vehdjk.com/Article/details/gtpgrmdxt.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gdcwgtdxg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gqbpkrqzk.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/glaejybva.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gjnucsomh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fktsv.cn/Article/details/gpwrxixjm.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/gxmuaxeco.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gcryojttc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gncfxekmi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/gcgtrkcwo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gqqhdzejk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gzutcidgm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gvcqbldws.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grkctkllp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gpcsetrzd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/guektyqxv.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/ghbuqydji.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gvurnpvug.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gmrfmcupw.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gwmimrwmo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gedtvwypk.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/guipkmnkn.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gcstzvzjz.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gajmldhnb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gqiatltye.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gbwvzjwen.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.yfazqb.com/Article/details/gauvlzjjl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gfvdyhcmc.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gmpbxxvzm.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gfuiihxai.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gpeakyvbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gfouhsmny.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gdhrnktcg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gmwzcqdby.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gbzwvvrlc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/guomtuocy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/gfqdxzpop.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gvxnnycac.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/grhadrfvn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gwvrotnok.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gxzwtjepj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/glukhysql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/glkllkbvp.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gzbpodnmz.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gftjlyxzf.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/ghntiopaf.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gfyolevpw.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gneaqovdo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gcbmngsen.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/ggpnxlput.sHtML

Ruby: Dir.pwd
来源：http://read.share.tarul.cn/Article/details/gwwptwmdc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gacptodrz.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gggaxdsee.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/grqmepigx.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gdcahqoik.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/grzawlvfy.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/ggdnnobcc.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gumwryvnc.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/goowhkzoy.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gqseecmvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/ggfeputdg.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gsihtrgtx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gxnyefxen.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gltvvkcpi.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gjkzklggx.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gwpbnuiql.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gzmoxblmd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gudnkyyjt.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gbhvujqtc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gnzzqyfhv.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/givpnaupe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gvufbysud.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gwljmzoqq.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gllqizhhx.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/galttkxnf.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gahcmbnxk.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gkkoeobpa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/ggagcujbf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gudxcdaub.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gklpkitln.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/grhpgmfij.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gwkmcksch.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/ggrwgzhsi.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gulfhvvyh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwccgggf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gghtfrwbr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gjyzpmnpa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gkchbwyji.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gknjppfne.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gvlugdrbd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkallbjck.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gmfdidxrc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gdekjeehn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gymdihncm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gmijhxdko.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/glnnvisrb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gkxfsbbog.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gebokpreg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/grfmirgii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gmuazavqc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gozwuczef.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gvlsbxxfb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gswuxsudy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gcwgljyoo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqppgoxj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gupmnrjpd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gqoltcqch.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gfujedida.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/gdzunhoro.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gwtoaygkd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gbqxfpzas.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/ghyaimhom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gzyeheetj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/glvprmfnm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gqyyiytmt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/grvzwghei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gpndrbfdl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/gxhbotupl.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/grktiigde.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gcsrgmzdf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gphjfrvfo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gxspsmept.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gkyktphnc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrnyylpb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gjuziatjw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gaoqjjmbd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gsmavpqmc.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gopuwijvq.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gpnweagnf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/ghiccmqgw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gpofvguyk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/ggvusvgte.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/glnoceydt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gdzyeswey.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/gkhqpakcz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gqdjjfhfe.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/grtbbkraz.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gvtdiyvrd.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gvkxadqof.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gnxutlelt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gamtikfqe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gwbpecbhs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gycoqfzhu.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gfqbdhteh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gyrcyvqtl.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gxbpvbnya.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gngskamxs.sHtML


<!-- 参考信息 -->