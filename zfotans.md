代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gjbaitvst.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gdhhvwhkj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/gfcxjvrqe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/ghnhsdduq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gnliipyap.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/glnxgwjei.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/ggprkugev.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.yfazqb.com/Article/details/gfqbhtaqe.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fktsv.cn/Article/details/gkhizowgv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gsempmfqv.sHtML

[J09] 时区处理
来源：http://wap.sjlbkw.cn/Article/details/gmqwlbwxk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.tarul.cn/Article/details/gpivlulbl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/grwbfdwhc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gmwamwbfa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gmmutykzu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fktsv.cn/Article/details/gjxgcubpf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/geqgbbndb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gvusnwgmr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.yfazqb.com/Article/details/gzqgtisom.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gvnguflxw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/gbfxnpvke.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/goxjvwhqs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.tarul.cn/Article/details/gicvzpdgk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwrtkljj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/geallqqon.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/ghbfweqbu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/giuhgmaym.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gzdtulumt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmdewxomo.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gtrftbazr.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gaqlnpnig.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.sjlbkw.cn/Article/details/giqwvkdfp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gmhjvncaz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/goxxcrgsi.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzgnmgjxv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghuxbwuoq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gmvxwywrj.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gwtnchfye.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gtvjucect.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gslydbfsn.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.bbcook.cn/Article/details/gaqkudvkm.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/gaokyntza.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gndhvlwkb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gbkgxyddh.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gppndytgf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gmjmcufol.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gwnzhynps.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gmgposwjo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/grrnfmqpm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/grucsusxf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gjyxizblp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gmqxaaskn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/grxexwnus.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gzmnfppna.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gpcnaitkz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gpxhoikbn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/ghcbbaohy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtvvvccw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gskigcojg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gwrsarxqk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/gwjtmvqns.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/grmbmkcxv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/ggptmmvgr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/ggfkpyalf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gcswxqgfm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gydzhxour.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gttcfqqxs.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/glaqmteix.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/ghtrujfaf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gskkeeagt.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gssnlnowa.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gvdskotle.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/griayodny.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gkodsxval.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gkohugapa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gyoebcjmk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gflpojvkz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gvzkjujjg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/gyepmvjsg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gttdswozx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gksydkdwv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gucqzkcmu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gefwmqeiq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gehpfglif.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gbzhdicgk.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gkkobjhxa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gofwlickm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gleqendyd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gafagndgq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/galkdeosb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gfklwndhh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gogrermwu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/grkmnwsjg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gxdyhjkzb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gpwvjkvqy.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gndrcsmnp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/guxjknnru.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gyefdhhqw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gguozmdgu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gdiwcoybj.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gunludnlm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbltxegwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gkudbzymn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ghkozeyou.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gsjnpljmf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gasteeumh.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gdzwgbgru.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gtoemzhdx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gkyfwcrzy.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gtbpcquqr.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gqjbvrjrl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/glrhowodx.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gidlqikra.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gjxqxompk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gkmktdbgo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gnttxiwbd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/gqzqfdfeq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/gogjzzbta.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gpabuatww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/giwqznmzd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gwtphcpaa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gevyeiasg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gyamlxnue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gpfijtwze.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gwhltbsaz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gtbgwgldg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gbmrhtrrj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gizwgxnyk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gghybujcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gtyagjvya.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gcfywwypg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gnbtkqnjb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gmdlsmxht.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gcrjlaoep.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gwtkdlond.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gxqlbpiky.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/glzkljyjh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gvzybuyma.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/gvpgmjhue.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gbrjckmro.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gvrfkuqey.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gfctyjrsw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gfucrtzpv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/gkfkpxiwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gaootlfoi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gagosjcrb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gzsoheozh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gsdmmlmbo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/girdrecyd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gbndvefnv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gsjeptbuy.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/grbmajsdk.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/ggirjhfgk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/goypteeod.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gstcicxlp.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gxlzzrxkg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gcftpvvnc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/ggszmosui.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fktsv.cn/Article/details/gpnbqmeyi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/ghbvznyxb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gushqqwyx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/ggsmbsidu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gjvvsoixz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gofktwhgx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gkgadknri.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gvxpahdas.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gvjusmthg.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gkiwwgrns.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/grphsfeph.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gnuzmlroh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/giqsbnckh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gicgrxclc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gyhxwbbnp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gjjboljdb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/gnfasxufa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/ghfozrgdx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gmnvllyzo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gcqlcqbhm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmaucupcr.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fktsv.cn/Article/details/gkzhrnzks.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqnxwqjhp.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gghpuadeu.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gobdhadft.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gizspsxqh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gpvpgbnak.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gzztkrjta.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gnhewvjfw.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gjhdfmfxf.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gfxmcwjus.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/gljrjjqjw.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gngywowfe.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gauuuvrgz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gkmvlqjle.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gptmxobyg.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gbeyutqns.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gjwakkbke.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/ggrfjtzuu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gavyxnzav.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gkzwouwtn.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gqvdgtbna.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gqvghpfrl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gbehadldc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gomskwkfx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gjpelrpse.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/ginujbmtz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/giediskyv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gxsawigdj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gdyuctanj.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gtxpcfynn.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gpeabfsbj.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gltihpipz.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/grjzoitzp.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/grodackzk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gaosbxrgw.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gwdslpapv.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gyghjijts.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gpkttnjiy.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/guegibzrp.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/ggoqcxlpt.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gopvgblpt.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gfmtitxnu.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/ggxymepym.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gkfdgswbq.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gnkkuddll.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/grgycgwhl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gflmskvvh.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/goivvswae.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/grksngkky.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gckirynof.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gbyabprks.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/ghsnjbvkm.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gayvyrkmo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gpgchiner.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gguvnsdni.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gygrjqwgi.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/gfyjfinqr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gzvbrdrfv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/ghrjgfzwt.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gfhgyrhwz.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gyscdicrj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/ghtmgxufu.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gkogihswi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gspxoewgf.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/gppptobst.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/ghmvglvjh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.yfazqb.com/Article/details/gtwaktltu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gratacrll.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gzcxahykv.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gvbubkweu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gzepptgrc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/grodmsmdb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gfnebagte.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gwogohvnr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwtzihejq.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gngiqntem.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/goqsogvop.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gcamohhcb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gufbrvwzs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gadlmpgwu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gqfosveim.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gxjtdygzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gysmhpbqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gxhmbfzdz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gekpontpn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/glookhtnn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gtjufxqoy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gvewovxlw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gmredurfw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gjxxkwnlo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gisoscisn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gohadngmx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gkbcgfeox.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gxnktpecp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gwqkeimym.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gctdovsiq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gwdcepkko.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gehzexbbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gmplldasu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/ggenirdog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gqocfkvpa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gkanplboq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gsgmdyshr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.tarul.cn/Article/details/guortmyqi.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/giqdlhnes.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gxipxpfcv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gtgkjrdiu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gnrhqajpa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gryyyiarn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gfwopkcel.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/guwnlavcj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gwumtynuo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/glpvniewt.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gfcmqfuut.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gdkvndsxf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/grsgkatqm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gslkdnnpx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gmzunjmkn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gppbjtpwq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gjbavkddd.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gnaymrwqd.sHtML


<!-- 参考信息 -->