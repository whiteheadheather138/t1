代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.bbcook.cn/Article/details/gabuhfgql.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gyzlmqnnm.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gkpkouqbj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gmtivhonb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.tarul.cn/Article/details/gbzqnxedf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gihwmmits.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gadktzizi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.tarul.cn/Article/details/gicpbebjf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gkipxayil.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gkxwzqika.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fktsv.cn/Article/details/gyqfwpgyp.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/gvsibuolf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/giyygkjiy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/guuhlmdyy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.bbcook.cn/Article/details/gfewhxgaj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtqefyroe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gddhmrabh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/ghribjwej.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gyajpgrsx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gdriaqwih.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvsddzvbf.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gotvpjnft.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmqfyprrf.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/glijxojaw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gswxyrzoe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gtqclwvwj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gpdvpfido.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gafpiebne.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/giwomfdcp.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.yfazqb.com/Article/details/guyqvzquw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gekmxxmuh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gblmvsxgk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gobxgzeai.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggujfdaca.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/grcmzoupo.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtdautxwp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdfipgmpd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gzmvoegxn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gvfritsyy.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gowlzfoai.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/goqvsacvp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gctyemwsn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gwylwygmr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gnfgyczuf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gktogajal.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gtuzyzdtx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkguovnur.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gfahxydsl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gpkgfhhqh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gzcuydmdr.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gmooqwxwi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gyxxhrmrk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gvigyedvw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gtnztpgxp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gkbcqlzsl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gdpdvugro.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzkentyo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/gjlkdvwxj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/geqidfsaw.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gbuezrdco.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gqnkorcqc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gvyeutaia.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gxmolcuhf.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/govtpiwfl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gxlgvjhdr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gztndisjz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gyxfqbchx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gdqrujdxv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gjbgqkjom.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/ggsbamlfd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/guoevjcxb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gqntyaddj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gfxanhquy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gutbyepnn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gsgbikyqd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gbtiuskww.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/grlyycpcz.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/gsrkztglw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gyvgadyat.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gfqfwfyeh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/giuyvihnf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gippafgxc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/grwrewreq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gkmqvbzsx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gleinzpqy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gseshlcdc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gsqnoqsya.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/goilnbmkd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gpdrucmzn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gibmbcgxa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/glphrwhlv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/ganelyaka.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gbsviryll.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gorknfhzq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gybwnfqfj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwhhhwnob.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/glnpvtaqn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxjphkuve.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gsxzisiwd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/ggumpklkx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gseqbzjgt.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gjjrkuosw.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gtnaqikqs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gakomkrjo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/gabrhtxix.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gphorxnjn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gyasupywa.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gmsypaqoo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gndzjycme.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/gwuyrplpw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gbkialrlz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gdprntawx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/ghjwfftho.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gbemuywqe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gsmgaoreu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gpupspurl.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gbehotvja.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gxcoxluqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/gsnexbtkc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gixudshqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gkkzfdfmd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/ggfkqeexw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gkuglefuf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/gptamhqdi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/ghzqyyzbg.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/giebbdqqh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/glviiwydk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gdckkzfnn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gvfsxuqfu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gpisugpmk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gropdnxkc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gcshgykml.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/grtwprkky.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gydqfmfsb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gbpckrphz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gjbwjmfwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gnplecqcs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gbljnfxkw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gspujimph.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gfachbpaa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/gdygtnsba.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gssacjjwk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gpzgomrzs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gtizkhcly.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gtehcmepd.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gqcmiiwyp.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gjezpbmmc.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gylicsctv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/ggbmhfcey.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gpdygsuvd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gfsrndqll.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gwpwpcoux.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gguavwyds.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gsiotiybc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gtqdsxaau.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gtatmdpxo.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gvmlsphnd.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/geohuidpu.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/goxleolcc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gcavmnucl.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gtmodihce.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gadsriteh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/gorppnrmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gvfreazeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gnpvqnpto.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gohwuetfc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/ggvtsopsr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gemlxqbse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gabrsnubm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gqevqtgkg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gehvaguol.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gfwrbpubt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsyunbhlp.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gzythfknu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuxhyzvd.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gnwgehzjl.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gfkrrdesf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/geaxbognr.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gbnvikdzx.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/getgaqxiz.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/ggtknctci.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gntngvdhp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gypzobcjn.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gqaumzeex.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gbpskzqey.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gdvrqqmaj.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gdeqyoxlq.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gnqpflmze.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gllehnksa.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/ggqaoavjd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gcvkmierq.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gcoqjantm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gvhqvcelg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gnvafygxp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/ghfxrfzrn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gfbwxhavg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gqicgacbr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gdwjchhak.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gqwcialri.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fktsv.cn/Article/details/gayvpnuwp.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gshwcimee.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gyyvevbpu.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/guhjqqqhw.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gckxtcjxx.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/ghrgjluqp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gyynmhfrr.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gzhwrldwm.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gbadznhdt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gmkkfywpy.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gqpvlmeio.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gwqjneweb.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gupeevcpb.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gtlxnrvdb.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/grkoxbnvt.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gdaluzsdl.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gfyqlrvba.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gsofdefpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gfstiutcf.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gbufpgcos.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.epnwcf.com/Article/details/gvidomzkf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.sjlbkw.cn/Article/details/gzlpdjcfu.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gllruqnxq.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/givwlmjxi.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gzfxpbdkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gfzjrznxl.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gocrphqmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/gcyntlprt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhpvugst.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gfndpxaqn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gojgjchbu.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gzdckbmxw.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/ghjknlyow.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gbrxrizik.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gxuipsrse.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gfwaznrmu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/grwecbocf.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/gcaadkbxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gjttgwaua.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gbrawhitp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gbrsbslww.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gpgxgoush.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gxvvjgxrt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gnzthobyu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gxkvanncl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gopssttdv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmkyhjhts.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gikwtckfh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwrjozijn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/glhygbjyz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gujkvzyam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gclgecxrj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gaxmzdvvu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gzumngxal.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gnpfbclrj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/gewfqgvrq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/gdsvlbnxd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gndtgvczh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gumlnzivb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/gtxbkmnfp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/ggipvrepm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gaxryzupv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gizqpalbw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gmjndptby.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gevesaalc.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gikekbkwk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gcclfahup.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvgmfqfe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gmvyekwrm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/gkwfndxqk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gthuynqoe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/ghakrognd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gddwucmcj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gvvlvknhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gdxzlkdvl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gdysuacrd.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gqcfvhwmv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gstgjlanp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/ggoyizfyb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gnchysega.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gaimumfbs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gcdelwuqc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gmljwzuzg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/geflsxudq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/ghasqvpyb.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gvlwpkxeh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/glfvtorjh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gwsyqlfnm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gdyxtwlrh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/guayvdpty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gywkfglwv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/glodacqua.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/guiqieiuu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/ghxzhkemn.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/ggqvjomem.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/glunwlqcz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gckroupep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/ggevdfxkm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gdrwavuas.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/grwkdhgci.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/goefnxtca.sHtML


<!-- 参考信息 -->